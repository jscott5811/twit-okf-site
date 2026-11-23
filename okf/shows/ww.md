---
type: show
title: "Windows Weekly"
description: "Windows Weekly (WW) transcript archive covering 286 official episodes (345–1010, 2014–2026) across 43 NotebookLM-ready Markdown chunks (8,642,595 words)."
tags: [twit, show, ww, windows-and-microsoft, android-and-mobile, apple-ecosystem]
generated:
  by: "antigravity/gemini-4-neon-medium"
  at: "2026-11-23T22:50:24Z"
sources:
  - id: "twit-show-page"
    resource: "https://twit.tv/shows/windows-weekly"
    title: "Official TWiT.tv show page for Windows Weekly"
  - id: "ww-md"
    resource: "local archive data/WW_Transcripts_*.md"
    title: "Windows Weekly processed Markdown transcript chunks (43 files)"
  - id: "ww-html"
    resource: "local archive data/WW_*.html"
    title: "Windows Weekly raw HTML transcript files (286 files)"
  - id: "show-map"
    resource: "local repo fetch_transcripts.py"
    title: "TWiT Transcript Archiver SHOW_MAP configuration"
  - id: "yt-catalog"
    resource: "local archive data_youtube/_catalog.json"
    title: "Discovered TWiT YouTube channel video catalog"
---

Windows Weekly is TWiT's flagship Microsoft and Windows roundtable covering Windows 10 and 11, Copilot, Microsoft 365, Azure, Xbox, Surface hardware, and enterprise computing. Launching **September 28, 2006** with its official show page at `https://twit.tv/shows/windows-weekly`,[^twit-show-page] **Windows Weekly** is tracked in `fetch_transcripts.py` under file prefix `WW`[^show-map] inside the [TWiT Transcript Archive](../datasets/twit-transcript-archive.md). The local archive holds **286** official HTML transcripts spanning episodes **345–1010** across **2014–2026**.[^ww-html]

Those official transcripts are compiled into **43** NotebookLM-ready Markdown chunks totaling **8,642,595 words** (averaging **30,218 words per episode**), preserving named speaker turns and episode metadata for research and quote extraction.[^ww-md] **Publication status:** Active on TWiT (hosted by Leo Laporte, Paul Thurrott, and Richard Campbell).[^twit-show-page]

Complete official episode-level index: [Windows Weekly Episodes (2014–2023)](../episodes/ww-2015-2023.md), [Windows Weekly Episodes (2024–2026)](../episodes/ww-2024-2026.md).[^ww-md]

## Quick Facts

| Field | Value |
| :--- | :--- |
| Show Name | Windows Weekly |
| Official Page | https://twit.tv/shows/windows-weekly |
| File Prefix | `WW` |
| Original Launch | September 28, 2006 |
| Publication Status | Active on TWiT (hosted by Leo Laporte, Paul Thurrott, and Richard Campbell) |
| Official HTML Transcripts | 286 |
| Processed Markdown Chunks | 43 |
| Total Official Words | 8,642,595 (avg 30,218 / ep) |
| Episode Range | 345–1010 |
| Years Covered | 2014–2026 |
| Primary Archived Voices | Paul Thurrott, Leo Laporte, Mary Jo Foley |
| YouTube Caption Backfill | 0 extracted / 394 numbered in YouTube catalog |

## History & Archive Evolution

Within the local archive, Windows Weekly spans **2014–2026** (8 dated calendar years), peaking in **2025** with **51** archived episodes (**1,725,109** words). The modern 2025–2026 era contributes **73** episodes (**2,462,341** words), reflecting TWiT's continuous publication of AI-assisted transcripts on `twit.tv`.[^ww-md]

### Year-by-Year Breakdown

| Year | Episodes | Words | Episode Range |
| :--- | ---: | ---: | :--- |
| 2014 | 41 | 931,393 | 345–390 |
| 2015 | 24 | 570,991 | 391–416 |
| 2021 | 3 | 85,415 | 753–755 |
| 2022 | 49 | 1,409,468 | 756–808 |
| 2023 | 48 | 1,603,806 | 810–860 |
| 2024 | 48 | 1,579,181 | 862–912 |
| 2025 | 51 | 1,725,109 | 894–964 |
| 2026 | 22 | 737,232 | 965–1010 |

Year-by-year counts derived from `data/WW_Transcripts_*.md` episode `**Date:**` headers.[^ww-md]

## Hosts & Regular Contributors

Transcript speaker-turn analysis across `WW_Transcripts_*.md` shows **Paul Thurrott** as the most frequent attributed voice (**191** episodes, **43,515** turns, active **2014–2026**), followed by **Leo Laporte** (**180** episodes, **34,130** turns, **2014–2026**). Other recurring voices in the archive include Mary Jo Foley, Richard Campbell, Leo, Paul. (Legacy transcripts occasionally record first-name-only labels such as `Leo` or `Steve` alongside full names.)[^ww-md]

| Speaker | Episodes Appeared | Speaker Turns | Active Date Span |
| :--- | ---: | ---: | :--- |
| [Paul Thurrott](../people/paul-thurrott.md) | 191 | 43,515 | 2014–2026 |
| [Leo Laporte](../people/leo-laporte.md) | 180 | 34,130 | 2014–2026 |
| Mary Jo Foley | 86 | 6,569 | 2014–2022 |
| [Richard Campbell](../people/richard-campbell.md) | 72 | 14,718 | 2015–2026 |
| Leo | 61 | 17,052 | 2014–2015 |
| Paul | 61 | 14,815 | 2014–2015 |
| Mary Jo | 59 | 7,016 | 2014–2022 |
| TWiT Intro | 31 | 34 | 2022–2023 |
| [Mikah Sargent](../people/mikah-sargent.md) | 18 | 1,318 | 2022–2026 |
| Rich Campbell | 15 | 3,404 | 2022–2023 |
| Daniel | 8 | 1,185 | 2014–2015 |
| Mary | 7 | 66 | 2014–2015 |
| Jo Foley | 7 | 7 | 2014–2015 |
| TWIT Intro | 7 | 7 | 2022–2023 |
| New Speaker | 6 | 7 | 2021–2022 |

Speaker statistics extracted strictly from structured speaker turns in `data/WW_Transcripts_*.md` (excluding unattributed YouTube captions).[^ww-md]

## Editorial Focus & Recurring Themes

Keyword and entity mining across all 286 official Windows Weekly transcripts confirms that coverage is anchored by [Windows & Microsoft](../topics/windows-and-microsoft.md) (65,680 mentions), [Android & Mobile](../topics/android-and-mobile.md) (12,555 mentions), [Apple Ecosystem](../topics/apple-ecosystem.md) (9,420 mentions).[^ww-md] At the product and organization level, the most heavily discussed subjects are **Windows** (25,092), **Microsoft** (22,586), **Google** (5,966), **Xbox** (5,410), **Apple** (4,999), **Windows 11** (3,399).[^ww-md]

Excluding `twit.tv` self-references and podcast sponsor reads, the show's most frequently cited external domains include `outlook.com` (118), `microsoft.com` (115), `allaboutmicrosoft.com` (113), `thurrott.com` (111), `leanpub.com` (105), reflecting the primary news sources, documentation hubs, and host blogs referenced on air.[^ww-md]

### Archive Topic Coverage

- [Windows & Microsoft](../topics/windows-and-microsoft.md) (65,680 mentions)
- [Android & Mobile](../topics/android-and-mobile.md) (12,555 mentions)
- [Apple Ecosystem](../topics/apple-ecosystem.md) (9,420 mentions)
- [AI & Machine Learning](../topics/ai-and-machine-learning.md) (5,413 mentions)
- [Hardware & Chips](../topics/hardware-and-chips.md) (4,755 mentions)
- [Tech Policy & Media](../topics/tech-policy-and-media.md) (4,481 mentions)

### Top Products, Tools & Entities

**Windows** (25,092), **Microsoft** (22,586), **Google** (5,966), **Xbox** (5,410), **Apple** (4,999), **Windows 11** (3,399), **Surface** (2,720), **Windows 10** (2,681), **Copilot** (2,581), **Android** (2,563), **Intel** (2,256), **Azure** (1,790).[^ww-md]

### Top Non-Sponsor External Domains

`outlook.com` (118), `microsoft.com` (115), `allaboutmicrosoft.com` (113), `thurrott.com` (111), `leanpub.com` (105), `sharefile.com` (90), `winsupersite.com` (75), `pub.com` (63), `throt.com` (46), `radio.com` (43).[^ww-md]

## Notable & Milestone Episodes

The milestones below highlight the chronological boundaries, longest transcript, and representative high-volume episodes in the Windows Weekly archive, paired with verbatim excerpts where clean attributed turns are present:[^ww-md]

- **Earliest archived episode:** Episode 345 (Jan 24th 2014) — *Windows Weekly 345 (Transcript)* (19,335 words, `WW_Transcripts_2014_345_355.md` — Keywords: Windows, Microsoft, Google, Chrome).[^ww-md]
  > "So we’re calling out right now. So if suddenly a woman in crisp starched white outfit with high heels and a giant nurse hat comes in you’ll forgive me if I swoon. Hello I’m the inoculator." — **Leo** [WW #345, Jan 24th 2014]
- **Latest archived episode:** Episode 1010 (Nov 18th 2026) — *Windows Weekly 1010 Transcript* (32,643 words, `WW_Transcripts_2026_1010_1010.md` — Keywords: Microsoft, Windows, Xbox, Google).[^ww-md]
  > "It's time for Windows Weekly. Paul Thurrott's here. Richard Campbell is back from his endless flight around the world. I think he's in Portugal today. We have lots to talk about." — **Leo Laporte** [WW #1010, Nov 18th 2026, TS:00:00:00]
- **Longest archived episode:** Episode 908 (Nov 20th 2024) — *Windows Weekly 908 Transcript* (47,548 words, `WW_Transcripts_2024_903_909.md` — Keywords: Windows, Microsoft, Xbox, Google).[^ww-md]
- **High-volume milestone episode #1:** Episode 356 (Apr 21st 2014) — *Windows Weekly 356 (Transcript)* (46,612 words, `WW_Transcripts_2014_356_364.md` — Keywords: Windows, Microsoft, Xbox, Apple).[^ww-md]
  > "It's time for Windows Weekly, the beer edition. (Laughs) Oh, baby! When you get Paul Thurrott and Mary Jo Foley in studio — you add Daniel Rubino from WP Central — to talk about this year's Build, you know you've got a great..." — **Laporte** [WW #356, Apr 21st 2014]
- **High-volume milestone episode #2:** Episode 810 (Jan 9th 2023) — *Windows Weekly Episode 810 Transcript* (45,171 words, `WW_Transcripts_2023_810_818.md` — Keywords: Windows, Microsoft, Google, Apple).[^ww-md]
  > "<laugh>. I did a couple of, uh, inadvertent splits and, uh, yeah. I felt like, ooh, I dodged a bullet there. Mm-hmm. <affirmative>, because, uh, there's nothing worse than Christmas than a groin pole injury. <laugh>." — **Leo Laporte** [WW #810, Jan 9th 2023, TS:00:04:06]

## Coverage Gaps & Backfill Status

Across the exhausted 241-page `twit.tv` transcript index, Windows Weekly has **344** pre-archive episodes before Episode 345 and **380** internal gaps between Episodes 345 and 1010.[^ww-html]

YouTube channel discovery (`data_youtube/_catalog.json`) identified **394** numbered episodes (717 total videos) on TWiT's official YouTube channel for Windows Weekly that can be selectively backfilled via `fetch_youtube_captions.py` (without speaker diarization).[^yt-catalog]

## See Also

- [TWiT Transcript Archive](../datasets/twit-transcript-archive.md) - Full dataset specification, NotebookLM chunking rules, and archive totals.
- [Windows Weekly Episodes (2014–2023)](../episodes/ww-2015-2023.md) - Complete episode-by-episode catalog for Windows Weekly.
- [Windows Weekly Episodes (2024–2026)](../episodes/ww-2024-2026.md) - Complete episode-by-episode catalog for Windows Weekly.
- [Windows & Microsoft Copilot Viewpoints](../viewpoints/windows-and-microsoft-copilot.md) - Cross-host viewpoint synthesis on this show's core domain.
- [Microsoft](../entities/microsoft.md) - Entity profile and mention trends across the TWiT archive.
- [OpenAI](../entities/openai.md) - Entity profile and mention trends across the TWiT archive.

[^twit-show-page]: Official TWiT.tv show page at `https://twit.tv/shows/windows-weekly` and TWiT program archive.
[^ww-md]: Processed Markdown chunks matching `data/WW_Transcripts_*.md` (43 files, 8,642,595 words).
[^ww-html]: Raw HTML transcript files matching `data/WW_*.html` (286 files).
[^show-map]: `SHOW_MAP` configuration in `fetch_transcripts.py` mapping `"windows weekly"` to `WW`.
[^yt-catalog]: Channel discovery inventory in `data_youtube/_catalog.json`.
