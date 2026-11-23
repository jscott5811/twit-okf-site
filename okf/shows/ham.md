---
type: show
title: "Ham Nation"
description: "Ham Nation (HAM) concluded its TWiT run on December 23, 2020 with 0 official transcripts across 241 crawled TWiT.tv pages, though 384 numbered episodes were discovered on YouTube."
tags: [twit, show, ham, unarchived, concluded-run]
generated:
  by: "antigravity/gemini-4-neon-medium"
  at: "2026-11-23T22:50:24Z"
sources:
  - id: "twit-show-page"
    resource: "https://twit.tv/shows/ham-nation"
    title: "Official TWiT.tv show page for Ham Nation"
  - id: "show-map"
    resource: "local repo fetch_transcripts.py"
    title: "TWiT Transcript Archiver SHOW_MAP configuration"
  - id: "list-pages"
    resource: "local archive data/transcripts_page_*.html"
    title: "Crawled TWiT.tv transcript index pages 1 through 241"
  - id: "yt-catalog"
    resource: "local archive data_youtube/_catalog.json"
    title: "Discovered TWiT YouTube channel video catalog"
---

Ham Nation is an amateur radio program covering ham radio gear, antennas, emergency communications, operating events, and community discussions. Premiering in **2011**, **Ham Nation** is registered in `SHOW_MAP` under file prefix `HAM`[^show-map] within the [TWiT Transcript Archive](../datasets/twit-transcript-archive.md) and has its official show page at `https://twit.tv/shows/ham-nation`.[^twit-show-page] Its TWiT network run concluded on **December 23, 2020** (Episode 485), after which the program continued via *Ham Radio Crash Course*.[^twit-show-page]

Across the complete 241-page crawl of `twit.tv/posts/transcripts` (`data/transcripts_page_1.html` through `data/transcripts_page_241.html`), **0 episodes** of Ham Nation were listed, leaving `data/` with 0 raw HTML transcripts and 0 processed Markdown chunks.[^list-pages] However, YouTube channel discovery (`data_youtube/_catalog.json`) identified **407** long-form videos (**384** numbered episodes) available for future unattributed YouTube caption backfill.[^yt-catalog]

## Quick Facts

| Field | Value |
| :--- | :--- |
| Show Name | Ham Nation |
| Official Page | https://twit.tv/shows/ham-nation |
| File Prefix | `HAM` |
| Original Launch | 2011 |
| Publication Status | Concluded TWiT run (final TWiT episode #485 aired December 23, 2020; later moved to Ham Radio Crash Course) |
| Official HTML Transcripts | 0 |
| Processed Markdown Chunks | 0 |
| Total Official Words | 0 |
| YouTube Catalog Discovered | 384 numbered episodes (407 total videos) |

## Coverage Gaps & Backfill Status

Because TWiT.tv's transcript index contains no entries for Ham Nation, the show currently has no speaker-attributed transcripts in `data/`.[^list-pages] Extracting English auto-captions from the **384** numbered episodes cataloged in `data_youtube/_catalog.json` via `fetch_youtube_captions.py` represents the primary path to bringing Ham Nation into the text archive, subject to the lack of speaker diarization in YouTube captions.[^yt-catalog]

## See Also

- [TWiT Transcript Archive](../datasets/twit-transcript-archive.md) - Full archive dataset specification, crawl scope, and completeness.
- [Sync and Process Archive Playbook](../playbooks/sync-and-process-archive.md) - CLI commands for official scraping and resumable YouTube caption backfill.
- [Hardware & Chips](../topics/hardware-and-chips.md) - Related electronics and hardware coverage across archived TWiT shows.

[^twit-show-page]: Official TWiT.tv program listing at `https://twit.tv/shows/ham-nation` and TWiT episode archive.
[^show-map]: `SHOW_MAP` entry `"ham nation": "HAM"` in `fetch_transcripts.py`.
[^list-pages]: Full 241-page crawl of `data/transcripts_page_1.html` through `data/transcripts_page_241.html`.
[^yt-catalog]: Channel discovery inventory in `data_youtube/_catalog.json`.
