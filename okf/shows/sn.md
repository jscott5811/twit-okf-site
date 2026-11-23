---
type: show
title: "Security Now"
description: "Security Now (SN) transcript archive covering 1,094 official episodes (1–1105, 2005–2026) across 332 NotebookLM-ready Markdown chunks (16,218,625 words)."
tags: [twit, show, sn, cybersecurity-and-privacy, windows-and-microsoft, android-and-mobile]
generated:
  by: "antigravity/gemini-4-neon-medium"
  at: "2026-11-23T21:34:55Z"
sources:
  - id: "sn-md"
    resource: "local archive data/SN_Transcripts_*.md"
    title: "Security Now processed Markdown transcript chunks (332 files)"
  - id: "sn-html"
    resource: "local archive data/SN_*.html"
    title: "Security Now raw HTML transcript files (1094 files)"
  - id: "show-map"
    resource: "local repo fetch_transcripts.py"
    title: "TWiT Transcript Archiver SHOW_MAP configuration"
  - id: "yt-catalog"
    resource: "local archive data_youtube/_catalog.json"
    title: "Discovered TWiT YouTube channel video catalog"
---

Security Now is TWiT's flagship deep-dive cybersecurity, cryptography, networking, and privacy podcast co-hosted by Steve Gibson and Leo Laporte, backed in this archive by both TWiT.tv transcripts and the historical GRC.com transcript back catalog. Tracked in `fetch_transcripts.py` under file prefix `SN`,[^show-map] **Security Now** is part of the [TWiT Transcript Archive](../datasets/twit-transcript-archive.md) and accounts for **1,094** official HTML transcripts spanning episodes **1–1105** across **2005–2026**.[^sn-html]

Those official transcripts are compiled into **332** NotebookLM-ready Markdown chunks totaling **16,218,625 words** (averaging **14,825 words per episode**), preserving named speaker turns and episode metadata for research and quote extraction.[^sn-md] The show's complete official episode-level index is available across [Security Now Episodes (2005–2010)](../episodes/sn-2005-2010.md), [Security Now Episodes (2011–2015)](../episodes/sn-2011-2015.md), [Security Now Episodes (2016–2020)](../episodes/sn-2016-2020.md), [Security Now Episodes (2021–2026)](../episodes/sn-2021-2026.md), [Security Now Episodes (Undated Legacy)](../episodes/sn-undated.md).[^sn-md]

## Quick Facts

| Field | Value |
| :--- | :--- |
| Show Name | Security Now |
| File Prefix | `SN` |
| Publication Status | Tracked in `SHOW_MAP` |
| Official HTML Transcripts | 1,094 |
| Processed Markdown Chunks | 332 |
| Total Official Words | 16,218,625 (avg 14,825 / ep) |
| Episode Range | 1–1105 |
| Years Covered | 2005–2026 |
| Primary Archived Voices | Steve Gibson, Steve, Description |
| YouTube Caption Backfill | 0 extracted / 400 numbered in YouTube catalog |

## History & Archive Evolution

Within the local archive, Security Now spans **2005–2026** (22 dated calendar years), peaking in **2008** with **53** archived episodes (**705,067** words). The modern 2025–2026 era contributes **40** episodes (**827,941** words), reflecting TWiT's continuous publication of AI-assisted transcripts on `twit.tv`. In addition, **572** episodes lack a parseable date header (primarily legacy GRC.com HTML files) and are grouped into undated episode-range chunks. Unlike other TWiT shows whose `twit.tv` transcripts begin in 2014 or 2021, Security Now achieves near-complete coverage back to **Episode 1 (2005)** because `fetch_transcripts.py` automatically backfills missing episodes from Steve Gibson's GRC.com archive.[^sn-md]

### Year-by-Year Breakdown

| Year | Episodes | Words | Episode Range |
| :--- | ---: | ---: | :--- |
| 2005 | 23 | 184,768 | 1–772 |
| 2006 | 43 | 373,280 | 21–72 |
| 2007 | 42 | 436,143 | 73–124 |
| 2008 | 53 | 705,067 | 125–816 |
| 2009 | 52 | 704,860 | 177–229 |
| 2010 | 48 | 624,615 | 230–981 |
| 2011 | 37 | 521,805 | 273–410 |
| 2012 | 17 | 232,831 | 335–869 |
| 2013 | 15 | 228,605 | 383–980 |
| 2014 | 18 | 290,067 | 316–471 |
| 2015 | 15 | 239,524 | 440–926 |
| 2016 | 14 | 241,053 | 543–724 |
| 2017 | 13 | 215,027 | 598–637 |
| 2018 | 13 | 190,592 | 626–697 |
| 2019 | 16 | 242,474 | 699–760 |
| 2020 | 19 | 275,438 | 566–836 |
| 2021 | 17 | 241,617 | 792–950 |
| 2022 | 11 | 161,794 | 851–900 |
| 2023 | 7 | 116,120 | 921–1052 |
| 2024 | 9 | 151,480 | 970–1006 |
| 2025 | 12 | 229,332 | 999–1058 |
| 2026 | 28 | 598,609 | 1045–1105 |
| Undated | 572 | 9,013,524 | 13–1095 |

Year-by-year counts derived from episode `**Date:**` headers in `data/SN_Transcripts_*.md`.[^sn-md]

## Hosts & Regular Contributors

Transcript speaker-turn analysis across `SN_Transcripts_*.md` shows **Steve Gibson** as the most frequent attributed voice (**1,093** episodes, **4,839** turns, active **2005–2026**), followed by **Steve** (**1,070** episodes, **126,662** turns, **2005–2026**). Other recurring voices in the archive include Description, Last Edit, Leo Laporte, Leo. (Note that legacy transcripts occasionally record first-name-only labels such as `Leo` or `Steve` alongside full names.)[^sn-md]

| Speaker | Episodes Appeared | Speaker Turns | Active Date Span |
| :--- | ---: | ---: | :--- |
| [Steve Gibson](../people/steve-gibson.md) | 1,093 | 4,839 | 2005–2026 |
| Steve | 1,070 | 126,662 | 2005–2026 |
| Description | 1,070 | 1,070 | 2005–2026 |
| Last Edit | 1,070 | 1,070 | 2005–2026 |
| [Leo Laporte](../people/leo-laporte.md) | 1,021 | 3,275 | 2005–2026 |
| Leo | 1,002 | 122,226 | 2005–2026 |
| SHOW TEASE | 729 | 729 | 2005–2026 |
| JASON | 25 | 1,246 | 2005–2022 |
| [JASON HOWELL](../people/jason-howell.md) | 24 | 24 | 2005–2022 |
| TOM MERRITT | 15 | 15 | 2011 |
| Finally | 12 | 12 | 2017 |
| FATHER ROBERT BALLECER | 12 | 12 | 2017 |
| MALE VOICE | 11 | 53 | 2013–2017 |
| PADRE | 10 | 1,130 | 2017 |
| Anyway | 9 | 9 | 2017–2025 |

Speaker statistics extracted strictly from structured speaker turns in `data/SN_Transcripts_*.md` (excluding unattributed YouTube captions).[^sn-md]

## Editorial Focus & Recurring Themes

Keyword and entity mining across all 1,094 official Security Now transcripts confirms that coverage is anchored by [Cybersecurity & Privacy](../topics/cybersecurity-and-privacy.md) (65,059 mentions), [Windows & Microsoft](../topics/windows-and-microsoft.md) (36,000 mentions), [Android & Mobile](../topics/android-and-mobile.md) (33,830 mentions).[^sn-md] At the product and organization level, the most heavily discussed subjects are **Windows** (16,001), **Microsoft** (14,930), **Google** (13,627), **SpinRite** (12,124), **Vulnerabilities** (10,964), **Apple** (8,273).[^sn-md]

Excluding `twit.tv` self-references and podcast sponsor reads, the show's most frequently cited external domains include `grc.com` (9,886), `google.com` (289), `aol.com` (193), `microsoft.com` (179), `amazon.com` (163), reflecting the primary news sources, documentation hubs, and host blogs referenced on air.[^sn-md]

### Archive Topic Coverage

- [Cybersecurity & Privacy](../topics/cybersecurity-and-privacy.md) (65,059 mentions)
- [Windows & Microsoft](../topics/windows-and-microsoft.md) (36,000 mentions)
- [Android & Mobile](../topics/android-and-mobile.md) (33,830 mentions)
- [Apple Ecosystem](../topics/apple-ecosystem.md) (14,928 mentions)
- [Linux & Open Source](../topics/linux-and-open-source.md) (11,671 mentions)
- [Tech Policy & Media](../topics/tech-policy-and-media.md) (11,520 mentions)

### Top Products, Tools & Entities

**Windows** (16,001), **Microsoft** (14,930), **Google** (13,627), **SpinRite** (12,124), **Vulnerabilities** (10,964), **Apple** (8,273), **Privacy** (7,823), **Encryption** (6,582), **Chrome** (5,899), **Firefox** (5,417), **Malware** (4,292), **Android** (3,532).[^sn-md]

### Top Non-Sponsor External Domains

`grc.com` (9,886), `google.com` (289), `aol.com` (193), `microsoft.com` (179), `amazon.com` (163), `paypal.com` (96), `twitter.com` (96), `youtube.com` (89), `github.com` (70), `polyfill.io` (66).[^sn-md]

## Notable & Milestone Episodes

The milestones below highlight the chronological boundaries, longest transcript, and representative high-volume episodes in the Security Now archive, paired with verbatim excerpts where clean attributed turns are present:[^sn-md]

- **Earliest archived episode:** Episode 1 (August 18, 2005) — *Security Now 1 Transcript* (3,780 words, `SN_Transcripts_2005_1_12.md` — Keywords: Windows, Firewall, Microsoft, Vulnerabilities).[^sn-md]
  > "How a never-disclosed Windows vulnerability was quickly reverse-engineered from the patches to fix it and turned into more than 12 potent and damaging Internet worms in three days." — **Description** [SN #1, August 18, 2005]
- **Latest archived episode:** Episode 1105 (Nov 17th 2026) — *Security Now 1105 transcript* (20,515 words, `SN_Transcripts_2026_1096_1105.md` — Keywords: Microsoft, Vulnerabilities, Windows, Google).[^sn-md]
  > "It's time for Security Now. Steve Gibson is here, and I have been waiting all week to find out what he thinks about the Microsoft Outlook outage, the FAA ground stop, the huge Patch Tuesday roller coaster, and, well, a whole lot..." — **Leo Laporte** [SN #1105, Nov 17th 2026, TS:00:00:00]
- **Longest archived episode:** Episode 1067 (Mar 3rd 2026) — *Security Now 1067 Transcript* (26,785 words, `SN_Transcripts_2026_1064_1074.md` — Keywords: CVE-2026-20127, Vulnerabilities, Meta, Apple).[^sn-md]
  > "Yeah. But except for that doesn't work so well when I do a show off schedule. Oh, everything's automated. In fact, I had to, because I was leaving town, I had to move all of my systemd services over to the framework, which stays..." — **Leo Laporte** [SN #1067, Mar 3rd 2026, TS:00:11:35]
- **High-volume milestone episode #1:** Episode 1081 (Unknown Date) — *Security Now 1081 Transcript* (25,921 words, `SN_Transcripts_1080-1084.md` — Keywords: CVE-2026-9082, Vulnerabilities, Claude, Microsoft).[^sn-md]
  > "This is Security Now! with Steve Gibson, Episode 1081, recorded Tuesday, June 2nd, 2026: "AI Captured the Flag." It's time for Security Now!, the show where we cover the latest security news, your privacy, how things work in the..." — **Leo Laporte** [SN #1081, Unknown Date]
- **High-volume milestone episode #2:** Episode 1021 (Unknown Date) — *Security Now 1021 Transcript* (25,443 words, `SN_Transcripts_1021-1022.md` — Keywords: Firefox, Apple, Windows, Android).[^sn-md]
  > "It's time for Security Now!. Steve Gibson is here. We're going to talk about, well, there's a lot of things. The 100-some fixes in Microsoft's Patch Tuesday last week. Why it's so difficult for Oracle to 'fess up. An Apple vs." — **SHOW TEASE** [SN #1021, Unknown Date]

## Coverage Gaps & Backfill Status

Across the exhausted 241-page `twit.tv` transcript index, Security Now has **0** pre-archive episodes before Episode 1 and **11** internal gaps between Episodes 1 and 1105. GRC.com auto-backfill fills nearly the entire 2005–2026 run (episodes 1–1105), leaving only 11 episodes unavailable on both `twit.tv` and GRC.com.[^sn-html]

YouTube channel discovery (`data_youtube/_catalog.json`) identified **400** numbered episodes (720 total videos) on TWiT's official YouTube channel for Security Now that can be selectively backfilled via `fetch_youtube_captions.py` (without speaker diarization).[^yt-catalog]

## See Also

- [TWiT Transcript Archive](../datasets/twit-transcript-archive.md) - Full dataset specification, NotebookLM chunking rules, and archive totals.
- [Security Now Episodes (2005–2010)](../episodes/sn-2005-2010.md) - Complete episode-by-episode catalog for Security Now.
- [Security Now Episodes (2011–2015)](../episodes/sn-2011-2015.md) - Complete episode-by-episode catalog for Security Now.
- [Security Now Episodes (2016–2020)](../episodes/sn-2016-2020.md) - Complete episode-by-episode catalog for Security Now.
- [Security Now Episodes (2021–2026)](../episodes/sn-2021-2026.md) - Complete episode-by-episode catalog for Security Now.
- [Security Now Episodes (Undated Legacy)](../episodes/sn-undated.md) - Complete episode-by-episode catalog for Security Now.
- [Cybersecurity & Privacy Viewpoints](../viewpoints/cybersecurity-and-privacy.md) - Cross-host viewpoint synthesis on this show's core domain.
- [GRC & Security Tools](../entities/grc-and-security-tools.md) - Entity profile and mention trends across the TWiT archive.
- [Microsoft](../entities/microsoft.md) - Entity profile and mention trends across the TWiT archive.
- [Mozilla & Open Web](../entities/mozilla-and-open-web.md) - Entity profile and mention trends across the TWiT archive.
- [EFF & Digital Rights](../entities/eff-and-digital-rights.md) - Entity profile and mention trends across the TWiT archive.

[^sn-md]: Processed Markdown chunks matching `data/SN_Transcripts_*.md` (332 files, 16,218,625 words).
[^sn-html]: Raw HTML transcript files matching `data/SN_*.html` (1,094 files).
[^show-map]: `SHOW_MAP` configuration in `fetch_transcripts.py` mapping `"security now"` to `SN`.
[^yt-catalog]: Channel discovery inventory in `data_youtube/_catalog.json`.
