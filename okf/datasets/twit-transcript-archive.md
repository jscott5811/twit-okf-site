---
type: dataset
title: "TWiT Transcript Archive"
description: "Complete local archive of 3,350 official TWiT.tv/GRC.com transcripts (577 NotebookLM-ready Markdown chunks, 64,082,577 words) plus 28 unattributed YouTube caption backfills."
tags: [dataset, transcripts, twit, markdown, notebooklm, youtube-captions, archive]
generated: { by: "antigravity/gemini-4-neon-medium", at: "2026-11-23T21:40:00Z" }
sources:
  - id: archive-data
    resource: "local archive data/*_Transcripts_*.md"
    title: "Processed official Markdown transcript chunks in data/ (577 files, 3,350 episodes)"
  - id: yt-data
    resource: "local archive data_youtube/*/*_yt.md"
    title: "YouTube caption backfill transcripts in data_youtube/ (28 files, unattributed)"
  - id: fetch-script
    resource: "local repo fetch_transcripts.py"
    title: "TWiT transcript scraper (fetch_transcripts.py)"
  - id: process-script
    resource: "local repo process_transcripts.py"
    title: "TWiT Markdown processor and chunker (process_transcripts.py)"
  - id: yt-script
    resource: "local repo fetch_youtube_captions.py"
    title: "YouTube caption backfill CLI (fetch_youtube_captions.py)"
  - id: twit-transcripts
    resource: https://twit.tv/posts/transcripts
    title: "TWiT.tv official transcript index"
  - id: grc-sn
    resource: https://www.grc.com/securitynow.htm
    title: "GRC.com Security Now transcript archive"
  - id: user-note
    resource: "user editorial note 2026-11-23"
    title: "User editorial note on concluded TWiT shows"
---

The **TWiT Transcript Archive** is a locally maintained, research-grade textual corpus documenting more than two decades of technology journalism, hardware analysis, cybersecurity reporting, and open-source discourse across the TWiT podcast network.[^archive-data][^twit-transcripts] Combining **official speaker-attributed transcripts** harvested from [TWiT.tv](https://twit.tv/posts/transcripts) (exhausting all 241 official index pages) and Steve Gibson's [GRC.com](https://www.grc.com/securitynow.htm) archive for [Security Now](../shows/sn.md) with **unattributed YouTube caption backfills** for pre-transcript episodes, the corpus spans **3,378 total episodes** and **57,346,125 spoken body words** (64,082,577 total file words across official Markdown chunks when speaker and timestamp prefixes are included).[^archive-data][^yt-data][^fetch-script][^grc-sn]

Designed both for longitudinal media research and for ingestion into retrieval-augmented tools such as Google NotebookLM and the repository's local FastAPI/React chat interface, the dataset separates high-trust attributed transcripts (`data/`) from unattributed automated YouTube captions (`data_youtube/`).[^process-script][^yt-script] Across the 18 show prefixes registered in `SHOW_MAP` inside `fetch_transcripts.py` and `process_transcripts.py`, 17 shows carry official downloaded transcripts in `data/`, while [Ham Nation](../shows/ham.md) (`HAM`) has zero official TWiT.tv transcripts across all 241 index pages but 383 missing numbered episodes cataloged on YouTube (407 total channel videos listed in `data_youtube/_catalog.json`).[^fetch-script][^process-script][^yt-script]

As an analytical foundation for this OKF v0.3 knowledge bundle, the archive captures a clear historical inflection in TWiT's publishing pipeline: early-era coverage (2005–2013) is anchored almost exclusively by GRC.com's verbatim [Security Now](../shows/sn.md) archive, followed by an initial multi-show transcription wave in 2014–2015, a sparser middle period in 2016–2020, and a massive network-wide expansion from 2022 through 2026 that peaks at 532 episodes and 8,651,521 spoken body words in 2025.[^archive-data]

## Quick Facts

| Attribute | Value |
|---|---|
| **Dataset Type** | Local multi-show podcast transcript corpus (HTML + NotebookLM Markdown)[^archive-data] |
| **Combined Indexed Episodes** | **3,378** (3,350 official attributed + 28 YouTube caption backfills)[^archive-data][^yt-data] |
| **Combined Spoken Body Words** | **57,346,125** (56,616,600 official + 729,525 YouTube captions)[^archive-data][^yt-data] |
| **Official Markdown File Words** | **64,082,577** across 577 chunk files (including `EP:/Date:/TS:/Speaker` prefixes)[^archive-data] |
| **Tracked Show Prefixes** | 18 in `SHOW_MAP` (17 active in `data/`; `HAM` official count = 0)[^fetch-script][^archive-data] |
| **Official Speaker Attribution** | 99.1% named speaker attribution in `data/`[^archive-data] |
| **Official Index Exhaustion** | 241 cached `twit.tv/posts/transcripts` listing pages[^fetch-script][^twit-transcripts] |
| **YouTube Backfill Catalog** | 2,696 missing numbered episodes discovered across 13 YouTube channels (`data_youtube/_catalog.json`)[^yt-script] |
| **Chunking Limits** | `MAX_WORDS = 250,000` / `MAX_BYTES = 100 MB` (largest chunk: 250,290 words / 1.47 MB)[^process-script][^archive-data] |
| **Operational Playbook** | [Sync and Process Archive](../playbooks/sync-and-process-archive.md) |

# Historical Evolution & Archive Eras

The temporal distribution of the TWiT Transcript Archive reflects the evolving transcription practices of both TWiT.tv and GRC.com rather than the raw broadcast output of the network.[^archive-data][^twit-transcripts][^grc-sn] Understanding these distinct coverage eras is essential when interpreting longitudinal mention counts across [Entities](../entities/index.md) and [Topics](../topics/index.md), because sharp year-over-year jumps often combine genuine editorial shifts (such as the post-2022 generative AI boom) with major expansions in transcript availability.[^archive-data]

During the **GRC Foundation Era (2005–2013)**, virtually the entire dated corpus consists of [Security Now](../shows/sn.md) episodes backfilled from `https://www.grc.com/sn/sn-{ep}.htm`, where [Steve Gibson](../people/steve-gibson.md) maintained complete verbatim transcripts from the show's inception.[^fetch-script][^grc-sn][^archive-data] Annual volume during this decade averages 15 to 53 dated episodes per year, supplemented by 560 undated (`year == 0`) episodes and 12 legacy GRC files whose date parser picked up pre-2005 historical dates mentioned in header text.[^archive-data][^process-script]

A **First Multi-Show Transcription Wave (2014–2015)** briefly broadened official TWiT.tv coverage to 7 active shows, yielding 273 episodes (4,243,302 spoken words) in 2014 and 176 episodes (3,134,442 spoken words) in 2015 before official site-wide transcription receded during the **Trough Era (2016–2020)**, when annual totals dropped to between 13 and 68 episodes across only 1 to 2 shows.[^archive-data]

Beginning in **2021** (33 episodes across 7 shows) and accelerating dramatically in **2022–2026**, TWiT.tv restored broad multi-show official transcription across 9 to 13 shows per year.[^archive-data] Annual output surged from 270 episodes (5.76 million spoken words) in 2022 to 341 episodes (7.57 million words) in 2023, 393 episodes (7.30 million words) in 2024, and an all-time archive peak of **532 episodes and 8,651,521 spoken body words across 13 active shows in 2025**, followed by 256 episodes (4,081,233 words) already indexed in 2026.[^archive-data]

## Year-by-Year Archive Volume

Spoken body word counts below exclude `EP:/Date:/TS:/Speaker` line prefixes (total official Markdown file word count including prefixes is 64,082,577 across 577 chunks).[^archive-data]

| Year | Episodes | Spoken Body Words | Active Shows |
|---|---|---|---|
| Pre-2005 (misparsed GRC dates) | 12 | 169,553 | 1 |
| 2005 | 24 | 171,237 | 2 |
| 2006 | 43 | 330,379 | 1 |
| 2007 | 42 | 397,514 | 1 |
| 2008 | 53 | 641,768 | 1 |
| 2009 | 52 | 635,116 | 1 |
| 2010 | 48 | 568,101 | 1 |
| 2011 | 37 | 477,243 | 1 |
| 2012 | 17 | 213,378 | 1 |
| 2013 | 15 | 205,550 | 1 |
| 2014 | 273 | 4,243,302 | 7 |
| 2015 | 176 | 3,134,442 | 7 |
| 2016 | 68 | 1,482,296 | 2 |
| 2017 | 57 | 1,181,665 | 2 |
| 2018 | 13 | 178,464 | 1 |
| 2019 | 16 | 226,854 | 1 |
| 2020 | 19 | 258,467 | 1 |
| 2021 | 33 | 625,077 | 7 |
| 2022 | 270 | 5,756,177 | 9 |
| 2023 | 341 | 7,573,691 | 10 |
| 2024 | 393 | 7,297,319 | 11 |
| 2025 | 532 | 8,651,521 | 13 |
| 2026 | 256 | 4,081,233 | 12 |
| Undated (year 0) | 560 | 8,116,253 | 1 |
| **Official Total (`data/`)** | **3,350** | **56,616,600** | **17** |
| **YouTube Caption Backfill (`data_youtube/`)** | **28** | **729,525** | **1** |
| **Combined Total** | **3,378** | **57,346,125** | **17** |

# Schema & Storage Architecture

The archive uses a two-stage file architecture on disk: raw scraped HTML pages and index listings are preserved as immutable source artifacts inside `data/`, while `process_transcripts.py` transforms them into clean, year-partitioned Markdown chunks sized comfortably below Google NotebookLM's 500,000-word and 200 MB per-source ceilings.[^fetch-script][^process-script] Unattributed YouTube captions are stored in a strictly separate directory tree (`data_youtube/`) so that downstream consumers never conflate diarized official transcripts with unattributed captions.[^yt-script][^yt-data]

## Directory File Patterns

| Pattern | Count | Description |
|---|---|---|
| `data/transcripts_page_<N>.html` | 241 | Exhausted TWiT.tv transcript listing pages (`N` = 1..241).[^fetch-script] |
| `data/<PREFIX>_<EP>.html` | 3,350 | Official raw episode HTML transcripts (plus occasional `<PREFIX>_unknown.html`).[^fetch-script] |
| `data/<PREFIX>_Transcripts_<YEAR>_<START>_<END>.md` | 432 | Year-split Markdown chunks generated with `--by-year`.[^process-script] |
| `data/<PREFIX>_Transcripts_<START>-<END>.md` | 145 | Fallback Markdown chunks when `year == 0` (primarily GRC.com Security Now back-catalog).[^process-script] |
| `data_youtube/<PREFIX>/<PREFIX>_<EP>_yt.md` | 28 | Unattributed YouTube caption Markdown transcripts (`diarization: "none (unattributed)"`).[^yt-data] |

## Markdown Episode & Line Format

Inside each official Markdown chunk, episodes are concatenated with horizontal-rule dividers (`---`) and standardized headers consisting of `# Episode: <title>` and `**Date:** <date_str>`.[^process-script] Every spoken turn is normalized into a structured line format (`EP:<num> Date:<YY-MM-DD> [TS:<timestamp>] - <Speaker> - <text>`, where the `TS:` token is included whenever source timestamps are present), achieving **99.1% named speaker attribution** across the 3,350 official episodes.[^process-script][^archive-data]

When `--by-year` is enabled, `process_transcripts.py` partitions each show's episodes by extracted calendar year and splits any oversized year into sequential episode-range chunks governed by `MAX_WORDS = 250,000` and `MAX_BYTES = 100 MB`.[^process-script] Across the current 577 official chunks, the largest single file measures 250,290 words (1.47 MB), ensuring full compatibility with NotebookLM and fast local keyword scoring.[^archive-data][^process-script]

## Tracked Shows (`SHOW_MAP`)

Both `fetch_transcripts.py` and `process_transcripts.py` define a canonical 18-show `SHOW_MAP` mapping lowercase TWiT title prefixes to uppercase file codes: `IM` ([Intelligent Machines](../shows/im.md)), `TWIG` ([This Week in Google](../shows/twig.md)), `WW` ([Windows Weekly](../shows/ww.md)), `MBW` ([Macbreak Weekly](../shows/mbw.md)), `TWIT` ([This Week in Tech](../shows/twit.md)), `SN` ([Security Now](../shows/sn.md)), `TWIS` ([This Week in Space](../shows/twis.md)), `TNW` ([Tech News Weekly](../shows/tnw.md)), `ULS` ([Untitled Linux Show](../shows/uls.md)), `HOT` ([Hands-On Tech](../shows/hot.md)), `HOW` ([Hands-On Windows](../shows/how.md)), `HOA` ([Hands-On Apple](../shows/hoa.md)), `KH` ([Know How](../shows/kh.md)), `BYB` ([Before You Buy](../shows/byb.md)), `IOS` ([iOS Today](../shows/ios.md)), `AAA` ([All About Android](../shows/aaa.md)), `FLOSS` ([FLOSS Weekly](../shows/floss.md)), and `HAM` ([Ham Nation](../shows/ham.md)).[^fetch-script][^process-script]

# YouTube Caption Backfill Pipeline

To quantify and gradually close historical gaps where TWiT.tv never published official transcripts, `fetch_youtube_captions.py` uses `yt-dlp --flat-playlist --dump-json` to inventory 13 official TWiT YouTube channels and compare every numbered video against existing `data/<PREFIX>_<EP>.html` files.[^yt-script] The cached catalog (`data_youtube/_catalog.json`) identified **2,696 missing numbered episodes** across those 13 channels, including deep pre-transcript backlogs for [All About Android](../shows/aaa.md) (394 missing), [Ham Nation](../shows/ham.md) (383 missing), [iOS Today](../shows/ios.md) (377 missing), [Macbreak Weekly](../shows/mbw.md) (373 missing), [Windows Weekly](../shows/ww.md) (366 missing), and [This Week in Tech](../shows/twit.md) (244 missing).[^yt-script]

During initial batch extraction via `youtube-transcript-api`, **28 episodes** of [This Week in Tech](../shows/twit.md) (`#3`, `#10`, and `#387`–`#412`, totaling **729,525 words**) were written to `data_youtube/TWIT/` before YouTube returned an `IpBlocked` rate-limit response and the script halted cleanly as designed.[^yt-data][^yt-script] Because YouTube auto-captions lack speaker diarization, every backfill file carries explicit `diarization: "none (unattributed)"` metadata, is cataloged separately in [YouTube Captions Catalog](../episodes/youtube-captions.md), and is strictly excluded from speaker-attributed [People](../people/index.md) and [Viewpoints](../viewpoints/index.md) analysis while remaining searchable for macro entity and topic trends.[^yt-data][^yt-script]

# Coverage Caveats & Data Hygiene

Researchers and agents consuming this dataset should account for four documented structural caveats:

- **GRC.com Security Now backfill:** Whenever `SN` is fetched, `fetch_transcripts.py` automatically downloads missing [Security Now](../shows/sn.md) episodes (`1..max_ep`) from `https://www.grc.com/sn/sn-{ep}.htm` (using 3-digit zero-padded IDs below episode 1000) and wraps the GRC table HTML into the standard parser format.[^fetch-script][^grc-sn]
- **Unparsed dates (`year == 0`) & legacy GRC date artifacts:** Exactly 145 chunks covering 560 episodes fall back to `{PREFIX}_Transcripts_{START}-{END}.md` naming when date extraction returns `0`, and 12 legacy GRC.com [Security Now](../shows/sn.md) files carry pre-2005 years parsed from historical references in the episode header.[^archive-data][^process-script]
- **Concluded shows (no longer publishing new episodes):** Per editorial confirmation recorded on 2026-11-23, three TWiT shows have completed their runs and are no longer publishing new episodes: [iOS Today](../shows/ios.md) (`IOS`, archived), [Hands-On Tech](../shows/hot.md) (`HOT`, archived), and **Home Theater Geeks** (not in `fetch_transcripts.py`'s `SHOW_MAP`; 0 transcripts in `data/`).[^user-note][^fetch-script]
- **Stale chunk cleanup before rebuilds:** Because chunk filenames encode start and end episode numbers (`<START>_<END>.md`), older `data/*_Transcripts_*.md` files must be removed before re-running `process_transcripts.py` so overlapping episode ranges do not duplicate word counts or search hits.[^process-script]

# See Also

- **Operations:** [Sync and Process Archive](../playbooks/sync-and-process-archive.md)
- **Catalogs & Directories:** [Shows](../shows/index.md), [Episodes](../episodes/index.md), [YouTube Captions Catalog](../episodes/youtube-captions.md)
- **Analytical Indexes:** [Entities](../entities/index.md), [Topics](../topics/index.md), [People](../people/index.md), [Viewpoints](../viewpoints/index.md)
- **Reference Tables:** [Notable People](../references/notable-people.md), [Organizations and Tools](../references/organizations-and-tools.md), [Publications and Newsletters](../references/publications-and-newsletters.md), [Recurring External Domains](../references/recurring-domains.md)

[^archive-data]: Processed official Markdown transcript chunks in data/ (577 files, 3,350 episodes)
[^yt-data]: YouTube caption backfill transcripts in data_youtube/ (28 files, unattributed)
[^fetch-script]: TWiT transcript scraper (fetch_transcripts.py)
[^process-script]: TWiT Markdown processor and chunker (process_transcripts.py)
[^yt-script]: YouTube caption backfill CLI (fetch_youtube_captions.py)
[^twit-transcripts]: TWiT.tv official transcript index
[^grc-sn]: GRC.com Security Now transcript archive
[^user-note]: User editorial note on concluded TWiT shows
