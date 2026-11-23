---
type: show
title: "MacBreak Weekly"
description: "MacBreak Weekly (MBW) transcript archive covering 259 official episodes (384–1065 (plus 1 unnumbered file), 2014–2026) across 37 NotebookLM-ready Markdown chunks (7,452,305 words)."
tags: [twit, show, mbw, apple-ecosystem, android-and-mobile, tech-policy-and-media]
generated:
  by: "antigravity/gemini-4-neon-medium"
  at: "2026-11-23T22:50:24Z"
sources:
  - id: "twit-show-page"
    resource: "https://twit.tv/shows/macbreak-weekly"
    title: "Official TWiT.tv show page for MacBreak Weekly"
  - id: "mbw-md"
    resource: "local archive data/MBW_Transcripts_*.md"
    title: "MacBreak Weekly processed Markdown transcript chunks (37 files)"
  - id: "mbw-html"
    resource: "local archive data/MBW_*.html"
    title: "MacBreak Weekly raw HTML transcript files (259 files)"
  - id: "show-map"
    resource: "local repo fetch_transcripts.py"
    title: "TWiT Transcript Archiver SHOW_MAP configuration"
  - id: "yt-catalog"
    resource: "local archive data_youtube/_catalog.json"
    title: "Discovered TWiT YouTube channel video catalog"
---

MacBreak Weekly is TWiT's flagship weekly Apple roundtable examining iPhone, Mac, iPad, Apple Silicon, macOS, Vision Pro, App Store regulation, and Apple's strategic direction. Launching **August 12, 2006** with its official show page at `https://twit.tv/shows/macbreak-weekly`,[^twit-show-page] **MacBreak Weekly** is tracked in `fetch_transcripts.py` under file prefix `MBW`[^show-map] inside the [TWiT Transcript Archive](../datasets/twit-transcript-archive.md). The local archive holds **259** official HTML transcripts spanning episodes **384–1065 (plus 1 unnumbered file)** across **2014–2026**.[^mbw-html]

Those official transcripts are compiled into **37** NotebookLM-ready Markdown chunks totaling **7,452,305 words** (averaging **28,773 words per episode**), preserving named speaker turns and episode metadata for research and quote extraction.[^mbw-md] **Publication status:** Active on TWiT (hosted by Leo Laporte with rotating Apple panelists).[^twit-show-page]

Complete official episode-level index: [MacBreak Weekly Episodes (2014–2023)](../episodes/mbw-2015-2023.md), [MacBreak Weekly Episodes (2024–2026)](../episodes/mbw-2024-2026.md).[^mbw-md]

## Quick Facts

| Field | Value |
| :--- | :--- |
| Show Name | MacBreak Weekly |
| Official Page | https://twit.tv/shows/macbreak-weekly |
| File Prefix | `MBW` |
| Original Launch | August 12, 2006 |
| Publication Status | Active on TWiT (hosted by Leo Laporte with rotating Apple panelists) |
| Official HTML Transcripts | 259 |
| Processed Markdown Chunks | 37 |
| Total Official Words | 7,452,305 (avg 28,773 / ep) |
| Episode Range | 384–1065 (plus 1 unnumbered file) |
| Years Covered | 2014–2026 |
| Primary Archived Voices | Leo Laporte, Andy Ihnatko, Alex Lindsay |
| YouTube Caption Backfill | 0 extracted / 399 numbered in YouTube catalog |

## History & Archive Evolution

Within the local archive, MacBreak Weekly spans **2014–2026** (8 dated calendar years), peaking in **2025** with **52** archived episodes (**1,582,826** words). The modern 2025–2026 era contributes **73** episodes (**2,227,304** words), reflecting TWiT's continuous publication of AI-assisted transcripts on `twit.tv`.[^mbw-md]

### Year-by-Year Breakdown

| Year | Episodes | Words | Episode Range |
| :--- | ---: | ---: | :--- |
| 2014 | 44 | 967,516 | 384–432 |
| 2015 | 22 | 588,498 | 430–456 |
| 2021 | 4 | 122,647 | 794–797 |
| 2022 | 24 | 723,926 | 798–827 |
| 2023 | 41 | 1,290,111 | 860–900 |
| 2024 | 51 | 1,532,303 | 902–953 |
| 2025 | 52 | 1,582,826 | 954–1005 |
| 2026 | 21 | 644,478 | 1006–1065 |

Year-by-year counts derived from `data/MBW_Transcripts_*.md` episode `**Date:**` headers.[^mbw-md]

## Hosts & Regular Contributors

Transcript speaker-turn analysis across `MBW_Transcripts_*.md` shows **Leo Laporte** as the most frequent attributed voice (**237** episodes, **34,325** turns, active **2014–2026**), followed by **Andy Ihnatko** (**227** episodes, **14,227** turns, **2014–2026**). Other recurring voices in the archive include Alex Lindsay, Jason Snell, Rene Ritchie, Andy. (Legacy transcripts occasionally record first-name-only labels such as `Leo` or `Steve` alongside full names.)[^mbw-md]

| Speaker | Episodes Appeared | Speaker Turns | Active Date Span |
| :--- | ---: | ---: | :--- |
| [Leo Laporte](../people/leo-laporte.md) | 237 | 34,325 | 2014–2026 |
| [Andy Ihnatko](../people/andy-ihnatko.md) | 227 | 14,227 | 2014–2026 |
| [Alex Lindsay](../people/alex-lindsay.md) | 187 | 14,305 | 2014–2025 |
| [Jason Snell](../people/jason-snell.md) | 144 | 13,966 | 2014–2026 |
| Rene Ritchie | 75 | 2,042 | 2014–2024 |
| Andy | 65 | 5,905 | 2014–2015 |
| Leo | 62 | 16,204 | 2014–2015 |
| Rene | 60 | 6,486 | 2014–2015 |
| [Mikah Sargent](../people/mikah-sargent.md) | 55 | 1,823 | 2021–2026 |
| Alex | 41 | 4,444 | 2014–2015 |
| Announcers | 27 | 27 | 2014–2015 |
| Chad | 25 | 163 | 2014–2015 |
| Jason | 23 | 1,125 | 2014–2015 |
| John Ashley | 20 | 51 | 2023–2026 |
| [Jason Howell](../people/jason-howell.md) | 16 | 34 | 2014–2023 |

Speaker statistics extracted strictly from structured speaker turns in `data/MBW_Transcripts_*.md` (excluding unattributed YouTube captions).[^mbw-md]

## Editorial Focus & Recurring Themes

Keyword and entity mining across all 259 official MacBreak Weekly transcripts confirms that coverage is anchored by [Apple Ecosystem](../topics/apple-ecosystem.md) (61,834 mentions), [Android & Mobile](../topics/android-and-mobile.md) (9,194 mentions), [Tech Policy & Media](../topics/tech-policy-and-media.md) (5,816 mentions).[^mbw-md] At the product and organization level, the most heavily discussed subjects are **Apple** (36,278), **iPhone** (7,311), **iPad** (5,254), **Google** (4,474), **iOS** (2,608), **Vision Pro** (2,445).[^mbw-md]

Excluding `twit.tv` self-references and podcast sponsor reads, the show's most frequently cited external domains include `sixcolors.com` (190), `imore.com` (167), `youtube.com` (119), `apple.com` (59), `1password.com` (56), reflecting the primary news sources, documentation hubs, and host blogs referenced on air.[^mbw-md]

### Archive Topic Coverage

- [Apple Ecosystem](../topics/apple-ecosystem.md) (61,834 mentions)
- [Android & Mobile](../topics/android-and-mobile.md) (9,194 mentions)
- [Tech Policy & Media](../topics/tech-policy-and-media.md) (5,816 mentions)
- [Windows & Microsoft](../topics/windows-and-microsoft.md) (3,374 mentions)
- [AI & Machine Learning](../topics/ai-and-machine-learning.md) (2,673 mentions)
- [Cybersecurity & Privacy](../topics/cybersecurity-and-privacy.md) (2,540 mentions)

### Top Products, Tools & Entities

**Apple** (36,278), **iPhone** (7,311), **iPad** (5,254), **Google** (4,474), **iOS** (2,608), **Vision Pro** (2,445), **MacBook** (2,256), **Android** (1,979), **YouTube** (1,954), **Apple Watch** (1,463), **Windows** (1,433), **App Store** (1,308).[^mbw-md]

### Top Non-Sponsor External Domains

`sixcolors.com` (190), `imore.com` (167), `youtube.com` (119), `apple.com` (59), `1password.com` (56), `99designs.com` (50), `news.org` (44), `shutterstock.com` (42), `hover.com` (37), `personalcapital.com` (36).[^mbw-md]

## Notable & Milestone Episodes

The milestones below highlight the chronological boundaries, longest transcript, and representative high-volume episodes in the MacBreak Weekly archive, paired with verbatim excerpts where clean attributed turns are present:[^mbw-md]

- **Earliest archived episode:** Episode 384 (Apr 2nd 2014) — *MacBreak Weekly 384 (Transcript)* (19,405 words, `MBW_Transcripts_2014_384_395.md` — Keywords: Apple, iPad, iPhone, iOS).[^mbw-md]
  > "Actually, it looks good. It looks really good now. Yeah. It's a beautiful African sunset. Oh, it was. Well I've brought you all here to discuss the latest hot news from Apple." — **Leo** [MBW #384, Apr 2nd 2014]
- **Latest archived episode:** Episode 1065 (Oct 13th 2026) — *MacBreak Weekly 1065 Transcript* (35,810 words, `MBW_Transcripts_2026_1047_1065.md` — Keywords: Apple, MacBook, iPhone, iPad).[^mbw-md]
  > "It's time for MacBreak Weekly. Andy, Jason, and Christina are all here, and yes, there's new Apple hardware. We're gonna talk about the HomeView, the new Apple HomePod Minis, the new Apple TV." — **Leo Laporte** [MBW #1065, Oct 13th 2026, TS:00:00:00]
- **Longest archived episode:** Episode 873 (Jun 7th 2023) — *MacBreak Weekly 873, Transcript* (46,844 words, `MBW_Transcripts_2023_868_874.md` — Keywords: Apple, iPad, iPhone, iOS).[^mbw-md]
  > "It's time for MacBreak Weekly. Andy Ihnatko's here. Alex Lindsay's here. And re just returned from the Apple Park campus. Mikah Sargent. Yes. We're gonna take a look at the Apple event yesterday." — **Leo Laporte** [MBW #873, Jun 7th 2023, TS:00:00:00]
- **High-volume milestone episode #1:** Episode 953 (Dec 22nd 2024) — *MacBreak Weekly 953 Transcript* (43,653 words, `MBW_Transcripts_2024_952_953.md` — Keywords: Apple, iPad, Vision Pro, iPhone).[^mbw-md]
  > "But I don't think I would ever again sit down to watch once YouTube TV, which isn't out yet for the headset. Youtube says it's on their roadmap, by the way, which is good news. Youtube TV is not. Oh, not YouTube TV. Youtube TV." — **Leo Laporte** [MBW #953, Dec 22nd 2024, TS:0:06:16]
- **High-volume milestone episode #2:** Episode 445 (May 31st 2015) — *MacBreak Weekly 445 (Transcript)* (42,434 words, `MBW_Transcripts_2015_445_453.md` — Keywords: Apple, MacBook, iPhone, Apple Watch).[^mbw-md]
  > "It's time for MacBreak Weekly, wow do we have a great show, a long one too. But listen to every minute because it's so good." — **Leo Laporte** [MBW #445, May 31st 2015]

## Coverage Gaps & Backfill Status

Across the exhausted 241-page `twit.tv` transcript index, MacBreak Weekly has **383** pre-archive episodes before Episode 384 and **424** internal gaps between Episodes 384 and 1065.[^mbw-html]

YouTube channel discovery (`data_youtube/_catalog.json`) identified **399** numbered episodes (720 total videos) on TWiT's official YouTube channel for MacBreak Weekly that can be selectively backfilled via `fetch_youtube_captions.py` (without speaker diarization).[^yt-catalog]

## See Also

- [TWiT Transcript Archive](../datasets/twit-transcript-archive.md) - Full dataset specification, NotebookLM chunking rules, and archive totals.
- [MacBreak Weekly Episodes (2014–2023)](../episodes/mbw-2015-2023.md) - Complete episode-by-episode catalog for MacBreak Weekly.
- [MacBreak Weekly Episodes (2024–2026)](../episodes/mbw-2024-2026.md) - Complete episode-by-episode catalog for MacBreak Weekly.
- [Apple Ecosystem & Antitrust Viewpoints](../viewpoints/apple-ecosystem-and-antitrust.md) - Cross-host viewpoint synthesis on this show's core domain.
- [Apple](../entities/apple.md) - Entity profile and mention trends across the TWiT archive.

[^twit-show-page]: Official TWiT.tv show page at `https://twit.tv/shows/macbreak-weekly` and TWiT program archive.
[^mbw-md]: Processed Markdown chunks matching `data/MBW_Transcripts_*.md` (37 files, 7,452,305 words).
[^mbw-html]: Raw HTML transcript files matching `data/MBW_*.html` (259 files).
[^show-map]: `SHOW_MAP` configuration in `fetch_transcripts.py` mapping `"macbreak weekly"` to `MBW`.
[^yt-catalog]: Channel discovery inventory in `data_youtube/_catalog.json`.
