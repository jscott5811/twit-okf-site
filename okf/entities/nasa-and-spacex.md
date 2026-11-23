---
type: entity
title: "NASA and SpaceX"
description: "Civil and commercial spaceflight leaders anchoring Mars exploration, Artemis lunar missions, Starship launches, and ISS operations."
tags: [entity, nasa, spacex, space, artemis]
generated: { by: "antigravity/gemini-4-neon-medium", at: "2026-11-23T21:40:00Z" }
sources:
  - id: archive-data
    resource: "local archive data/*_Transcripts_*.md"
    title: "Processed official TWiT transcript Markdown chunks (577 files, 3,350 episodes)"
  - id: yt-data
    resource: "local archive data_youtube/*/*_yt.md"
    title: "YouTube caption backfill transcripts (28 files, unattributed)"
  - id: dataset-doc
    resource: /datasets/twit-transcript-archive.md
    title: "TWiT Transcript Archive dataset specification"
---

**NASA and SpaceX** is the centerpiece institutional pairing of spaceflight coverage in the [TWiT Transcript Archive](../datasets/twit-transcript-archive.md), accumulating **5,056 combined mentions**—comprising **5,029 official transcript mentions** across 13 of 17 active shows and **27 unattributed YouTube caption backfill mentions**.[^archive-data][^yt-data][^dataset-doc] Together, the U.S. civil space agency and the leading commercial launch provider anchor the network's reporting on Artemis lunar architecture, Mars sample return and settlement planning, International Space Station (ISS) crew transport, Starship orbital test flights, and Starlink satellite constellations.

While spaceflight was an occasional curiosity on general TWiT talk shows during the 2010s, the launch and transcription of *This Week in Space* (`TWIS`) transformed NASA and SpaceX into a major weekly editorial beat. Hosted by space author [Rod Pyle](../people/rod-pyle.md) and Space.com editor-in-chief [Tariq Malik](../people/tariq-malik.md), the show pairs technical mission tracking with candid policy reporting—examining how NASA's Commercial Crew and Artemis programs rely on SpaceX's rapid hardware iteration even as federal budget battles, administrator nominations, and political friction test the public-private partnership.[^archive-data]

| Quick Facts | Value |
|---|---|
| **Entity Type** | Entity (Civil Space Agency & Commercial Spaceflight) |
| **Combined Mentions** | 5,056 |
| **Official Transcript Mentions** | 5,029 |
| **YouTube Backfill Mentions** | 27 |
| **Active Show Coverage** | 13 of 17 shows (76.5%) |
| **Top Show** | [This Week in Space](../shows/twis.md) (3,696 official mentions; 73.5%) |
| **2025–2026 Official Share** | 2,598 mentions (51.7% of official total) |
| **Peak Dated Year (2020–2026)** | 2025 (1,905 mentions) |

# Historical Arc & Year-by-Year Trajectory

The chronological curve of **NASA and SpaceX** is one of the steepest late-stage ramps in the archive, reflecting both commercial spaceflight milestones and the addition of `TWIS` transcripts to the corpus.[^archive-data] Across the entire pre-2020 official archive, the entity recorded just **151 mentions**, followed by **1 in 2020** and **14 in 2021**—before TWiT had a dedicated transcribed spaceflight show in the dataset.

Mentions rose to **248 in 2022** and **223 in 2023** before surging more than sevenfold to **1,682 in 2024** (bringing 2020–2024 to **2,168 official mentions**).[^archive-data] That 2024 inflection coincided with continuous `TWIS` coverage of Boeing Starliner's troubled crewed test flight and uncrewed return, SpaceX's Starship Super Heavy booster tower catch, and NASA's deliberations over Mars Sample Return and the VIPER lunar rover.

The **2025–2026** period accounts for more than half of the entity's official footprint: **2,598 mentions** (**51.7%** of the official total), peaking at **1,905 in 2025** and continuing at **693 in 2026**.[^archive-data] Coverage during 2025 centered on proposed NASA budget cuts analyzed with the Planetary Society, political friction between Elon Musk and Donald Trump, and Jared Isaacman's candidacy for NASA administrator. Only **112 mentions** appear in undated (`year == 0`) official transcripts, alongside **27** in the YouTube caption backfill.[^archive-data][^yt-data]

| Period | Mentions |
|---|---|
| Pre-2020 (official) | 151 |
| 2020 | 1 |
| 2021 | 14 |
| 2022 | 248 |
| 2023 | 223 |
| 2024 | 1,682 |
| 2025 | 1,905 |
| 2026 | 693 |
| Undated (year 0) | 112 |
| YouTube Caption Backfill (`data_youtube/`) | 27 |

# Cross-Show Editorial Coverage

Coverage of **NASA and SpaceX** is heavily concentrated in its specialist home, *This Week in Space* (`TWIS`), which generates **3,696 official mentions** (**73.5%** of the archive total).[^archive-data] Every episode pairs mission play-by-play with interviews of space journalists (Ars Technica's Eric Berger, Space.com's Mike Wall), planetary scientists (Jim Bell), and policy advocates (the Planetary Society's Casey Dreier).

*This Week in Tech* (`TWIT`) ranks second with **599 mentions** (11.9%), covering major SpaceX milestones, Elon Musk's ventures, and Starlink's telecom disruption. A middle tier—*Security Now* (`SN`, **167**), *This Week in Google* (`TWIG`, **167**), and *Macbreak Weekly* (`MBW`, **139**)—picks up the entity when satellite internet security, direct-to-cell connectivity, or NASA technology partnerships intersect with their core beats. Eight remaining shows (`TNW`, `WW`, `IM`, `IOS`, `FLOSS`, `AAA`, `KH`, `ULS`) contribute a combined 261 mentions, while four shows (`BYB`, `HOA`, `HOT`, `HOW`) record zero mentions.

| Show | Mentions |
|---|---|
| [This Week in Space](../shows/twis.md) (`TWIS`) | 3,696 |
| [This Week in Tech](../shows/twit.md) (`TWIT`) | 599 |
| [Security Now](../shows/sn.md) (`SN`) | 167 |
| [This Week in Google](../shows/twig.md) (`TWIG`) | 167 |
| [Macbreak Weekly](../shows/mbw.md) (`MBW`) | 139 |
| [Tech News Weekly](../shows/tnw.md) (`TNW`) | 67 |
| [Windows Weekly](../shows/ww.md) (`WW`) | 60 |
| [Intelligent Machines](../shows/im.md) (`IM`) | 57 |
| [iOS Today](../shows/ios.md) (`IOS`) | 25 |
| [FLOSS Weekly](../shows/floss.md) (`FLOSS`) | 23 |
| [All About Android](../shows/aaa.md) (`AAA`) | 13 |
| [Know How](../shows/kh.md) (`KH`) | 9 |
| [Untitled Linux Show](../shows/uls.md) (`ULS`) | 7 |

# Products, Sub-Topics & Recurring Debates

The co-occurring sub-topic breakdown illustrates the dual structure of civil science and commercial launch infrastructure.[^archive-data] **NASA** leads with **3,422 official mentions**—more than double **SpaceX** (**1,607**)—while **Mars** ranks second overall at **2,370 mentions**, underscoring how deeply both NASA's robotic science missions and SpaceX's settlement ambitions animate the archive.

On the hardware side, **Starship** (**861 mentions**) and **Artemis** (**758 mentions**) anchor debates over humanity's return to the Moon and transit to Mars. Hosts and guests repeatedly contrast SpaceX's rapid hardware iteration against legacy aerospace contractors: on `TWIS #128` (Sep 13th 2024), discussing Boeing Starliner's uncrewed return, Tariq Malik emphasized the corporate gulf separating traditional defense primes from SpaceX, while on `TWIS #136` (Nov 8th 2024), Eric Berger noted a Chinese company proposed its own rocket-catching tower within a week of SpaceX's Starship booster catch.

**Starlink** (**526**) and **Falcon 9** (**111**) represent SpaceX's operational workhorses alongside Commercial Crew Dragon flights. Meanwhile, NASA governance and funding form a recurring policy debate: `TWIS #164` (Jun 6th 2025) dissected an austere NASA budget request alongside the survival of the Roman Space Telescope, and `TWIS #188` (Dec 7th 2025) analyzed Jared Isaacman's renewed candidacy to lead NASA.[^archive-data]

| Product / Sub-Topic | Official Mentions |
|---|---|
| NASA | 3,422 |
| Mars | 2,370 |
| SpaceX | 1,607 |
| Starship | 861 |
| Artemis | 758 |
| Starlink | 526 |
| Falcon 9 | 111 |

# Landmark & Highest-Density Episodes

All eight highest-density episodes are `This Week in Space` broadcasts recorded between June 2024 and December 2025.[^archive-data]

- **Starliner vs. Starship & Mars Science (`TWIS #114`, `TWIS #128`, `TWIS #130`):** `TWIS #114` (Jun 7th 2024; **69 mentions**) paired coverage of Starliner and Starship flight tests. Three months later, `TWIS #128` (Sep 13th 2024; **70 mentions**) examined Starliner's uncrewed return:
  > "I just want to make it really clear that I think that the fundamental issue that for what we're seeing when we compare it to the SpaceX which is of the world, is that there it's a very different company." — Tariq Malik `[This Week in Space #128, Sep 13th 2024, TS:00:42:41]`
  Two weeks later, `TWIS #130` (Sep 27th 2024; **70 mentions**) welcomed planetary scientist Jim Bell on Mars Sample Return, VIPER, and SpaceX's 2026 Starship-to-Mars target.
- **The Starship Tower Catch (`TWIS #136`):** The densest episode in the archive is `TWIS #136` (Nov 8th 2024; **84 mentions**), featuring Rod Pyle, Tariq Malik, and Eric Berger:
  > "Literally within a week of the Starship tower catch, which was so preposterous, Right... Within a week of that, a Chinese company had a proposal out to get funding to develop their own tower catching, you know, rocket catching tower." — Eric Berger `[This Week in Space #136, Nov 8th 2024, TS:00:38:22]`
- **NASA Budget Crisis & Leadership Drama (`TWIS #164`, `TWIS #188`):** `TWIS #164` (Jun 6th 2025; **78 mentions**) brought in Casey Dreier on NASA's proposed budget cuts and Musk–Trump friction:
  > "Yeah, and you just named out Jim Bridenstine, trump's NASA administrator at the time, as like the shepherd for that, naming the Artemis program, naming the Roman space telescope, which also got a pass surprisingly after being canceled." — Tariq Malik `[This Week in Space #164, Jun 6th 2025, TS:01:07:43]`
  Six months later, `TWIS #188` (Dec 7th 2025; **73 mentions**) paired Tariq Malik with Space.com's Mike Wall on Jared Isaacman's renewed bid for NASA administrator.

| Show | Episode | Date | Title | Mentions |
|---|---|---|---|---|
| [This Week in Space](../shows/twis.md) | #136 | Nov 8th 2024 | This Week in Space 136 Transcript | 84 |
| [This Week in Space](../shows/twis.md) | #164 | Jun 6th 2025 | This Week in Space 164 Transcript | 78 |
| [This Week in Space](../shows/twis.md) | #188 | Dec 7th 2025 | This Week in Space 188 Transcript | 73 |
| [This Week in Space](../shows/twis.md) | #128 | Sep 13th 2024 | This Week in Space 128 Transcript | 70 |
| [This Week in Space](../shows/twis.md) | #130 | Sep 27th 2024 | This Week in Space 130 Transcript | 70 |
| [This Week in Space](../shows/twis.md) | #114 | Jun 7th 2024 | This Week in Space 114 Transcript | 69 |
| [This Week in Space](../shows/twis.md) | #139 | Dec 7th 2024 | This Week in Space 139 Transcript | 68 |
| [This Week in Space](../shows/twis.md) | #158 | Apr 25th 2025 | This Week in Space 158 Transcript | 66 |

# Archive Methodology & Caveats

Statistics derive from **577 official processed transcript chunks** (3,350 attributed episodes) and **28 unattributed YouTube caption backfill files** documented in the [TWiT Transcript Archive](../datasets/twit-transcript-archive.md) specification.[^archive-data][^yt-data][^dataset-doc] Official transcripts account for **5,029** of **5,056** combined mentions (99.5%). The sharp 2024–2025 ramp reflects both major spaceflight milestones and expanded `TWIS` transcript coverage; **112 official mentions** reside in `Undated (year 0)` legacy transcripts, and some automated 2024–2025 `TWIS` transcripts contain minor numeric speaker-diarization artifacts without affecting attributed host or guest quotes.

# See Also

- **Topics:** [Space and Science](../topics/space-and-science.md), [Android and Mobile](../topics/android-and-mobile.md), [Hardware and Chips](../topics/hardware-and-chips.md)
- **Viewpoints:** [Space Exploration and Commercial Space](../viewpoints/space-exploration-and-commercial-space.md)
- **Related Entities:** [Google](../entities/google.md), [Apple](../entities/apple.md), [Meta and Social Platforms](../entities/meta-and-social-platforms.md)
- **Key Voices:** [Rod Pyle](../people/rod-pyle.md), [Tariq Malik](../people/tariq-malik.md), [Leo Laporte](../people/leo-laporte.md)
- **Dataset & References:** [TWiT Transcript Archive](../datasets/twit-transcript-archive.md), [Organizations and Tools](../references/organizations-and-tools.md)

[^archive-data]: Processed official TWiT transcript Markdown chunks (577 files, 3,350 episodes)
[^yt-data]: YouTube caption backfill transcripts (28 files, unattributed)
[^dataset-doc]: TWiT Transcript Archive dataset specification
