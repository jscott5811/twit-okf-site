---
type: show
title: "Tech News Weekly"
description: "Tech News Weekly (TNW) transcript archive covering 182 official episodes (215–464, 2022–2026) across 11 NotebookLM-ready Markdown chunks (2,190,660 words)."
tags: [twit, show, tnw, apple-ecosystem, android-and-mobile, tech-policy-and-media]
generated:
  by: "antigravity/gemini-4-neon-medium"
  at: "2026-11-23T21:34:55Z"
sources:
  - id: "tnw-md"
    resource: "local archive data/TNW_Transcripts_*.md"
    title: "Tech News Weekly processed Markdown transcript chunks (11 files)"
  - id: "tnw-html"
    resource: "local archive data/TNW_*.html"
    title: "Tech News Weekly raw HTML transcript files (182 files)"
  - id: "show-map"
    resource: "local repo fetch_transcripts.py"
    title: "TWiT Transcript Archiver SHOW_MAP configuration"
  - id: "yt-catalog"
    resource: "local archive data_youtube/_catalog.json"
    title: "Discovered TWiT YouTube channel video catalog"
---

Tech News Weekly is TWiT's weekly technology journalism program featuring interviews with reporters, researchers, and analysts behind the week's biggest stories in AI, big tech, hardware, and digital policy. Tracked in `fetch_transcripts.py` under file prefix `TNW`,[^show-map] **Tech News Weekly** is part of the [TWiT Transcript Archive](../datasets/twit-transcript-archive.md) and accounts for **182** official HTML transcripts spanning episodes **215–464** across **2022–2026**.[^tnw-html]

Those official transcripts are compiled into **11** NotebookLM-ready Markdown chunks totaling **2,190,660 words** (averaging **12,036 words per episode**), preserving named speaker turns and episode metadata for research and quote extraction.[^tnw-md] The show's complete official episode-level index is available across [Tech News Weekly Episodes](../episodes/tnw.md).[^tnw-md]

## Quick Facts

| Field | Value |
| :--- | :--- |
| Show Name | Tech News Weekly |
| File Prefix | `TNW` |
| Publication Status | Tracked in `SHOW_MAP` |
| Official HTML Transcripts | 182 |
| Processed Markdown Chunks | 11 |
| Total Official Words | 2,190,660 (avg 12,036 / ep) |
| Episode Range | 215–464 |
| Years Covered | 2022–2026 |
| Primary Archived Voices | Mikah Sargent, Jason Howell, Jennifer Pattison Tuohy |
| YouTube Caption Backfill | 0 extracted / 50 numbered in YouTube catalog |

## History & Archive Evolution

Within the local archive, Tech News Weekly spans **2022–2026** (5 dated calendar years), peaking in **2025** with **51** archived episodes (**602,577** words). The modern 2025–2026 era contributes **73** episodes (**845,707** words), reflecting TWiT's continuous publication of AI-assisted transcripts on `twit.tv`.[^tnw-md]

### Year-by-Year Breakdown

| Year | Episodes | Words | Episode Range |
| :--- | ---: | ---: | :--- |
| 2022 | 24 | 281,599 | 215–244 |
| 2023 | 36 | 485,053 | 280–316 |
| 2024 | 49 | 578,301 | 318–367 |
| 2025 | 51 | 602,577 | 368–418 |
| 2026 | 22 | 243,130 | 419–464 |

Year-by-year counts derived from episode `**Date:**` headers in `data/TNW_Transcripts_*.md`.[^tnw-md]

## Hosts & Regular Contributors

Transcript speaker-turn analysis across `TNW_Transcripts_*.md` shows **Mikah Sargent** as the most frequent attributed voice (**157** episodes, **6,795** turns, active **2022–2026**), followed by **Jason Howell** (**55** episodes, **2,095** turns, **2022–2025**). Other recurring voices in the archive include Jennifer Pattison Tuohy, Leo Laporte, Dan Moren, Abrar Al-Heeti. (Note that legacy transcripts occasionally record first-name-only labels such as `Leo` or `Steve` alongside full names.)[^tnw-md]

| Speaker | Episodes Appeared | Speaker Turns | Active Date Span |
| :--- | ---: | ---: | :--- |
| [Mikah Sargent](../people/mikah-sargent.md) | 157 | 6,795 | 2022–2026 |
| [Jason Howell](../people/jason-howell.md) | 55 | 2,095 | 2022–2025 |
| Jennifer Pattison Tuohy | 30 | 895 | 2023–2026 |
| [Leo Laporte](../people/leo-laporte.md) | 28 | 47 | 2023–2025 |
| Dan Moren | 27 | 544 | 2022–2026 |
| Abrar Al-Heeti | 25 | 617 | 2023–2026 |
| Amanda Silberling | 24 | 393 | 2022–2026 |
| [Rod Pyle](../people/rod-pyle.md) | 15 | 70 | 2022–2026 |
| Emily Forlini | 14 | 453 | 2024–2026 |
| Ant Pruitt | 14 | 189 | 2022–2023 |
| Scott Stein | 12 | 258 | 2024–2026 |
| [Mark Gurman](../people/mark-gurman.md) | 9 | 117 | 2022–2025 |
| Scott Wilkinson | 9 | 45 | 2022–2024 |
| Emily Dreibelbis | 8 | 181 | 2023–2024 |
| Jacob Ward | 7 | 344 | 2025–2026 |

Speaker statistics extracted strictly from structured speaker turns in `data/TNW_Transcripts_*.md` (excluding unattributed YouTube captions).[^tnw-md]

## Editorial Focus & Recurring Themes

Keyword and entity mining across all 182 official Tech News Weekly transcripts confirms that coverage is anchored by [Apple Ecosystem](../topics/apple-ecosystem.md) (6,400 mentions), [Android & Mobile](../topics/android-and-mobile.md) (4,221 mentions), [Tech Policy & Media](../topics/tech-policy-and-media.md) (3,573 mentions).[^tnw-md] At the product and organization level, the most heavily discussed subjects are **Apple** (3,313), **Google** (2,406), **Microsoft** (1,000), **Amazon** (965), **iPhone** (781), **Android** (638).[^tnw-md]

Excluding `twit.tv` self-references and podcast sponsor reads, the show's most frequently cited external domains include `checkout.com` (48), `vpn.com` (28), `cnet.com` (22), `bitwarden.com` (21), `theverge.com` (20), reflecting the primary news sources, documentation hubs, and host blogs referenced on air.[^tnw-md]

### Archive Topic Coverage

- [Apple Ecosystem](../topics/apple-ecosystem.md) (6,400 mentions)
- [Android & Mobile](../topics/android-and-mobile.md) (4,221 mentions)
- [Tech Policy & Media](../topics/tech-policy-and-media.md) (3,573 mentions)
- [AI & Machine Learning](../topics/ai-and-machine-learning.md) (2,381 mentions)
- [Windows & Microsoft](../topics/windows-and-microsoft.md) (2,137 mentions)
- [Cybersecurity & Privacy](../topics/cybersecurity-and-privacy.md) (1,990 mentions)

### Top Products, Tools & Entities

**Apple** (3,313), **Google** (2,406), **Microsoft** (1,000), **Amazon** (965), **iPhone** (781), **Android** (638), **Meta** (627), **Privacy** (607), **TikTok** (599), **Smart Home** (535), **iOS** (531), **Windows** (473).[^tnw-md]

### Top Non-Sponsor External Domains

`checkout.com` (48), `vpn.com` (28), `cnet.com` (22), `bitwarden.com` (21), `theverge.com` (20), `discourse.org` (17), `v-e-e-a-m.com` (16), `progress.com` (15), `sixcolors.com` (14), `mylio.com` (14).[^tnw-md]

## Notable & Milestone Episodes

The milestones below highlight the chronological boundaries, longest transcript, and representative high-volume episodes in the Tech News Weekly archive, paired with verbatim excerpts where clean attributed turns are present:[^tnw-md]

- **Earliest archived episode:** Episode 215 (Jan 5th 2022) — *Tech News Weekly Episode 215 Transcript* (20,772 words, `TNW_Transcripts_2022_215_240.md` — Keywords: TikTok, Apple, Amazon, Android).[^tnw-md]
  > "Hello and happy almost new year. I am Mikah Sargent and Jason Howell and I have put together the best interviews of the year for Tech News Weekly. We have got a lot to talk about, including anybody remember lawyer cat." — **Mikah Sargent** [TNW #215, Jan 5th 2022, TS:00:00:00]
- **Latest archived episode:** Episode 464 (Nov 19th 2026) — *Tech News Weekly 464 Transcript* (11,999 words, `TNW_Transcripts_2026_419_464.md` — Keywords: Xbox, Amazon, iPhone, EFF).[^tnw-md]
  > "Coming up on Tech News Weekly, Jennifer Pattison Tuohy of The Verge is here. GTA 6 is also here, and 2 non-gamers talk about it. It's, it's me and Jen." — **Mikah Sargent** [TNW #464, Nov 19th 2026, TS:00:00:00]
- **Longest archived episode:** Episode 215 (Jan 5th 2022) — *Tech News Weekly Episode 215 Transcript* (20,772 words, `TNW_Transcripts_2022_215_240.md` — Keywords: TikTok, Apple, Amazon, Android).[^tnw-md]
  > "Hello and happy almost new year. I am Mikah Sargent and Jason Howell and I have put together the best interviews of the year for Tech News Weekly. We have got a lot to talk about, including anybody remember lawyer cat." — **Mikah Sargent** [TNW #215, Jan 5th 2022, TS:00:00:00]
- **High-volume milestone episode #1:** Episode 367 (Dec 18th 2024) — *Tech News Weekly 367 Transcript* (17,941 words, `TNW_Transcripts_2024_361_367.md` — Keywords: Google, Apple, Passkeys, Microsoft).[^tnw-md]
  > "And so it begins. So, before we get into the results of the experiment, could you tell us a bit about the process Like what generative AI systems did you use? It sounds like chat GPT from OpenAI." — **Mikah Sargent** [TNW #367, Dec 18th 2024, TS:0:03:48]
- **High-volume milestone episode #2:** Episode 432 (Apr 9th 2026) — *Tech News Weekly 432 Transcript* (17,681 words, `TNW_Transcripts_2026_419_464.md` — Keywords: Google, Apple, Artemis, ChatGPT).[^tnw-md]
  > "Coming up on Tech News Weekly, Amanda Silberling of TechCrunch is here we talk about Google's AI overviews. It's a New York Times piece looking at the accuracy of the tool as well as a question of AI's use in journalism." — **Mikah Sargent** [TNW #432, Apr 9th 2026, TS:00:00:00]

## Coverage Gaps & Backfill Status

Across the exhausted 241-page `twit.tv` transcript index, Tech News Weekly has **214** pre-archive episodes before Episode 215 and **68** internal gaps between Episodes 215 and 464.[^tnw-html]

YouTube channel discovery (`data_youtube/_catalog.json`) identified **50** numbered episodes (50 total videos) on TWiT's official YouTube channel for Tech News Weekly that can be selectively backfilled via `fetch_youtube_captions.py` (without speaker diarization).[^yt-catalog]

## See Also

- [TWiT Transcript Archive](../datasets/twit-transcript-archive.md) - Full dataset specification, NotebookLM chunking rules, and archive totals.
- [Tech News Weekly Episodes](../episodes/tnw.md) - Complete episode-by-episode catalog for Tech News Weekly.
- [Apple](../entities/apple.md) - Entity profile and mention trends across the TWiT archive.
- [Google](../entities/google.md) - Entity profile and mention trends across the TWiT archive.
- [OpenAI](../entities/openai.md) - Entity profile and mention trends across the TWiT archive.
- [Meta & Social Platforms](../entities/meta-and-social-platforms.md) - Entity profile and mention trends across the TWiT archive.

[^tnw-md]: Processed Markdown chunks matching `data/TNW_Transcripts_*.md` (11 files, 2,190,660 words).
[^tnw-html]: Raw HTML transcript files matching `data/TNW_*.html` (182 files).
[^show-map]: `SHOW_MAP` configuration in `fetch_transcripts.py` mapping `"tech news weekly"` to `TNW`.
[^yt-catalog]: Channel discovery inventory in `data_youtube/_catalog.json`.
