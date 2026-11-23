---
type: playbook
title: "Sync and Process Archive"
description: "Operational procedure for fetching official TWiT.tv/GRC.com transcripts, backfilling YouTube captions, cleaning stale chunks, regenerating NotebookLM-ready Markdown files, and querying via the local webapp."
tags: [playbook, sync, cli, webapp, scraping, processing, youtube-captions]
generated: { by: "antigravity/gemini-4-neon-medium", at: "2026-11-23T21:40:00Z" }
sources:
  - id: readme
    resource: "local repo README.md"
    title: "TWiT Transcript Archiver README"
  - id: fetch-script
    resource: "local repo fetch_transcripts.py"
    title: "TWiT transcript scraper (fetch_transcripts.py)"
  - id: process-script
    resource: "local repo process_transcripts.py"
    title: "TWiT Markdown processor and chunker (process_transcripts.py)"
  - id: yt-script
    resource: "local repo fetch_youtube_captions.py"
    title: "YouTube caption backfill CLI (fetch_youtube_captions.py)"
  - id: webapp-server
    resource: "local repo webapp/server/main.py"
    title: "Local FastAPI backend (webapp/server/main.py)"
  - id: webapp-client
    resource: "local repo webapp/client/src/App.jsx"
    title: "Local React frontend (webapp/client/src/App.jsx)"
---

**Sync and Process Archive** is the canonical operational runbook for maintaining the [TWiT Transcript Archive](../datasets/twit-transcript-archive.md), spanning official HTML transcript harvesting from TWiT.tv and GRC.com, stale Markdown chunk cleanup, NotebookLM-compatible year-split chunk generation, respectful YouTube caption backfilling, and interactive querying through the local FastAPI/React web application.[^readme][^fetch-script][^process-script][^yt-script][^webapp-server]

The workflow is engineered for idempotency and rate-limit safety on Windows (where the Python CLI toolchain is recommended over optional Go binaries).[^readme][^fetch-script] Existing raw `.html` files in `data/` and existing `_yt.md` files in `data_youtube/` are automatically skipped on subsequent runs, while cached listing pages beyond page 5 prevent redundant scraping of static historical index pages unless `--refresh-list` is explicitly passed.[^fetch-script][^yt-script]

## Quick Reference

| Stage | Primary Script / Service | Input | Output | Key Safety Control |
|---|---|---|---|---|
| **1. Official Fetch** | `fetch_transcripts.py` | `twit.tv/posts/transcripts` & `grc.com` | `data/<PREFIX>_<EP>.html`, `data/transcripts_page_<N>.html` | `--throttle 3.0` (avoids HTTP 418)[^fetch-script] |
| **2. Stale Cleanup** | Manual / Webapp `/api/process` | `data/*_Transcripts_*.md` | Clean `data/` (preserves `.html`) | Never delete raw `.html` files[^process-script][^webapp-server] |
| **3. Chunk Processing** | `process_transcripts.py` | `data/<PREFIX>_<EP>.html` | `data/<PREFIX>_Transcripts_*.md` | `MAX_WORDS = 250,000` / `100 MB`[^process-script] |
| **4. YouTube Backfill** | `fetch_youtube_captions.py` | 13 TWiT YouTube channels | `data_youtube/_catalog.json`, `data_youtube/<PREFIX>/*_yt.md` | Halts cleanly on `429` / `IpBlocked`[^yt-script] |
| **5. Local Webapp** | `webapp/server/main.py` + Vite UI | `data/*_Transcripts_*.md` | Port `8001` API + Chat UI | 900,000-char context budget[^webapp-server][^webapp-client] |

# Trigger & Preconditions

Run this procedure whenever refreshing the [TWiT Transcript Archive](../datasets/twit-transcript-archive.md) with newly published episodes, recovering historical pre-transcript episodes via YouTube captions, regenerating NotebookLM-ready Markdown chunks after parser updates, or preparing the corpus for local RAG chat queries.[^readme][^fetch-script][^yt-script]

Before starting, confirm that Python 3 is available in the repository root (`twit-transcript-archiver/`), that `youtube-transcript-api` and `yt-dlp` are installed if running YouTube caption discovery or extraction, and that a Gemini API key is available if using the webapp's Chat Assistant tab.[^yt-script][^webapp-server]

# Step-by-Step Procedure

## 1. Fetch Official Transcripts (`fetch_transcripts.py`)

`fetch_transcripts.py` scrapes the TWiT.tv transcript listing pages (currently extending to page 241), matches show titles against its 18-entry `SHOW_MAP`, downloads missing episode HTML files into `data/<PREFIX>_<EP>.html`, and automatically backfills missing [Security Now](../shows/sn.md) episodes from GRC.com whenever `SN` is included.[^fetch-script] Pages 1 through 5 are always fetched fresh to catch new episodes, whereas pages `> 5` are served from `data/transcripts_page_<N>.html` unless `--refresh-list` is supplied.[^fetch-script]

- **Full archive sync across all 18 shows (uses cached index pages `> 5`):**
  ```bash
  python -u fetch_transcripts.py --all --pages 250 --throttle 3.0
  ```
- **Force-refresh all index pages (keep `--throttle 3.0` to avoid `twit.tv` HTTP 418 rate limits):**
  ```bash
  python -u fetch_transcripts.py --all --refresh-list --pages 250 --throttle 3.0
  ```
- **Fetch specific shows using positional arguments** (note: `README.md` mentions `--shows`, but `fetch_transcripts.py` actually accepts positional show codes or show names):[^readme][^fetch-script]
  ```bash
  python -u fetch_transcripts.py TWIT SN --pages 250 --throttle 3.0
  ```
- **Optional explicit GRC.com [Security Now](../shows/sn.md) range backfill:** pass `--grc-sn-range 1-1105` to target a specific episode span directly from `https://www.grc.com/sn/sn-{ep}.htm`.[^fetch-script]

## 2. Remove Stale Markdown Chunks

Before regenerating Markdown chunks, delete existing `data/*_Transcripts_*.md` files while keeping all raw `data/*.html` files intact.[^process-script][^webapp-server] Because chunk filenames encode the first and last episode number in each chunk (`<PREFIX>_Transcripts_<YEAR>_<START>_<END>.md`), adding new episodes shifts the filename boundary; leaving older chunks on disk causes duplicate episodes and inflated counts during search or NotebookLM ingestion.[^process-script]

## 3. Process HTML into NotebookLM Markdown Chunks (`process_transcripts.py`)

`process_transcripts.py` parses each show's raw HTML files, normalizes speaker lines into `EP:<num> Date:<YY-MM-DD> [TS:<timestamp>] - <Speaker> - <text>`, extracts publication years (falling back to `year == 0` when unparseable), and writes year-split Markdown chunks capped at `MAX_WORDS = 250,000` and `MAX_BYTES = 100 MB`.[^process-script]

- **Process all downloaded shows split by calendar year:**
  ```bash
  python -u process_transcripts.py --all --by-year
  ```
- **Process specific shows using positional arguments** (note: `README.md` mentions `--prefixes`, but `process_transcripts.py` accepts positional show codes or show names):[^readme][^process-script]
  ```bash
  python -u process_transcripts.py --by-year IM TWIG
  ```

## 4. Backfill Missing Pre-Transcript Episodes via YouTube Captions (`fetch_youtube_captions.py`)

For episodes never transcribed on TWiT.tv, `fetch_youtube_captions.py` separates discovery from caption downloads so that large channel inventories only need to be fetched once and caption extraction can resume safely across sessions.[^yt-script]

- **Discover missing numbered episodes across all 13 official TWiT YouTube channels** (caches inventory in `data_youtube/_catalog.json`; currently 2,696 missing numbered episodes discovered across `TWIT`, `WW`, `MBW`, `FLOSS`, `IOS`, `AAA`, `TNW`, `TWIS`, `SN`, `HOT`, `HOW`, `HAM`, and `ULS`):[^yt-script]
  ```bash
  python -u fetch_youtube_captions.py --all --discover-only
  ```
- **Resume caption extraction in respectful batches using the cached catalog** (automatically halts cleanly on any YouTube `429`, `Too Many Requests`, `RequestBlocked`, `IpBlocked`, or CAPTCHA signal; never attempts to bypass bot gates):[^yt-script]
  ```bash
  python -u fetch_youtube_captions.py --all --use-cache --throttle 10.0 --max-downloads 20
  ```
- **Provenance isolation:** Extracted files are written to `data_youtube/<PREFIX>/<PREFIX>_<EP>_yt.md` with explicit `source: youtube-captions` and `diarization: "none (unattributed)"` headers, keeping them completely isolated from speaker-attributed official transcripts in `data/`.[^yt-script]

## 5. Operate and Query via the Local Webapp

The repository includes a local FastAPI backend (`webapp/server/main.py`) and React/Vite frontend (`webapp/client/src/App.jsx`) that wrap both CLI scripts and provide an archive-grounded chat interface.[^webapp-server][^webapp-client]

1. **Start the services:** Launch the FastAPI backend with `python webapp/server/main.py` (listening on port `8001`) and start the Vite frontend with `npm run dev` inside `webapp/client`.[^webapp-server]
2. **Trigger fetches from the UI:** Select specific shows or toggle **ALL SHOWS** (default `200` pages), optionally enable **Force refresh list index** (`--refresh-list`), and click **Fetch Transcripts** (`POST /api/fetch`), which streams unbuffered `fetch_transcripts.py` logs and parses page/download progress.[^webapp-client][^webapp-server]
3. **Rebuild chunks from the UI:** Click **Process for Chat**, which automatically clears stale `*_Transcripts_*.md` files and invokes `process_transcripts.py --all --by-year` with real-time progress streaming.[^webapp-server]
4. **Query the archive in Chat Assistant:** Supply a Gemini API key in the Chat Assistant tab; `POST /api/chat` scores `.md` chunks and individual episodes by keyword, show, and year relevance up to a **900,000-character context budget** and forwards conversation history to the model.[^webapp-server][^webapp-client]

# Troubleshooting & Operational Caveats

- **HTTP 418 / Rate Limiting on TWiT.tv:** Always maintain `--throttle 3.0` (or higher) when performing deep or refreshed index scans; avoid lowering throttle values during multi-page backfills.[^fetch-script]
- **YouTube `IpBlocked` / `429` Stops:** Encountering `IpBlocked` is expected during extended caption runs; wait before resuming with `--use-cache --throttle 10.0 --max-downloads 20`, and never use proxies or CAPTCHA workarounds.[^yt-script]
- **README Flag Discrepancy:** Ignore the legacy `--shows` and `--prefixes` examples in `README.md` when invoking the Python scripts directly; both `fetch_transcripts.py` and `process_transcripts.py` parse show codes as positional arguments.[^readme][^fetch-script][^process-script]
- **Concluded Shows:** New fetches will no longer yield fresh official episodes for concluded shows such as [iOS Today](../shows/ios.md) and [Hands-On Tech](../shows/hot.md), though historical YouTube caption backfills remain cataloged in `data_youtube/_catalog.json`.[^yt-script]

# See Also

- **Dataset Specification:** [TWiT Transcript Archive](../datasets/twit-transcript-archive.md)
- **Catalogs:** [Shows](../shows/index.md), [Episodes](../episodes/index.md), [YouTube Captions Catalog](../episodes/youtube-captions.md)

[^readme]: TWiT Transcript Archiver README
[^fetch-script]: TWiT transcript scraper (fetch_transcripts.py)
[^process-script]: TWiT Markdown processor and chunker (process_transcripts.py)
[^yt-script]: YouTube caption backfill CLI (fetch_youtube_captions.py)
[^webapp-server]: Local FastAPI backend (webapp/server/main.py)
[^webapp-client]: Local React frontend (webapp/client/src/App.jsx)
