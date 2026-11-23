---
type: reference
title: "Recurring External Domains"
description: "Top non-sponsor external websites and domains mentioned across all 577 official TWiT transcript chunks and 28 YouTube caption backfills, with filtered sponsor domains documented."
tags: [reference, domains, links, websites, sponsors, archive]
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

**Recurring External Domains** catalogs the 25 most frequently spoken and referenced non-sponsor websites across all **3,350 official attributed episodes** (577 Markdown chunks) and **28 unattributed YouTube caption backfills** in the [TWiT Transcript Archive](../datasets/twit-transcript-archive.md).[^archive-data][^yt-data][^dataset-doc] Whereas [Publications and Newsletters](../references/publications-and-newsletters.md) tracks editorial brand names, this domain-level index captures explicit URLs spoken aloud during show segments, tool recommendations, show-note pointers, and host sign-offs.[^archive-data]

By an order of magnitude, **`grc.com`** dominates the entire archive with **9,893 official mentions** (across 3 shows, plus 2 in YouTube backfills), reflecting [Steve Gibson](../people/steve-gibson.md)'s two-decade habit of pointing [Security Now](../shows/sn.md) listeners to Gibson Research Corporation show notes, SpinRite pages, ShieldsUP, and security utilities.[^archive-data] Behind `grc.com`, major consumer web platforms—`youtube.com` (537 official + 49 YouTube backfill across 13 shows), `google.com` (518 across 12 shows), `microsoft.com` (305 across 7 shows), `amazon.com` (246 across 9 shows), and `apple.com` (149 across 9 shows)—form the core infrastructure layer of spoken web references.[^archive-data][^yt-data]

The 2025–2026 column also captures two vivid real-time shifts in internet culture and TWiT's host ecosystem: first, the near-complete domain migration from **`twitter.com`** (182 all-time official mentions, dropping to just 5 in 2025–2026) to **`x.com`** (243 all-time, with 170—or 70.0%—occurring in 2025–2026 across 6 shows); and second, the prominence of **host-owned personal and vertical domains** such as `space.com` (251 of 354 in 2025–2026), `sixcolors.com` (123 of 267), `leanpub.com` (43 of 108), `pylebooks.com` (28 of 29), `jeffjarvis.com` (26 of 26), `runasradio.com` (24 of 30), `nss.org` (21 of 23), and `adastramagazine.com` (21 of 23).[^archive-data]

## Quick Facts

| Metric | Value |
|---|---|
| **Cataloged Non-Sponsor Domains** | **25** top recurring external websites[^archive-data] |
| **Most Referenced Domain** | `grc.com` — 9,893 official mentions (3 shows) + 2 YouTube backfill[^archive-data][^yt-data] |
| **Broadest Cross-Show Domain** | `youtube.com` — 537 official mentions across 13/17 shows (+ 49 YouTube backfill)[^archive-data][^yt-data] |
| **Top Developer & Archival Domains** | `github.com` (97 across 11 shows), `archive.org` (85 across 9 shows)[^archive-data] |
| **Platform Rebrand Signal** | `x.com` (170 in 2025–2026) vs. `twitter.com` (5 in 2025–2026)[^archive-data] |
| **Filtered Noise Categories** | Self-links (`twit.tv`, `twi.tv`), transcript footers (`temi.com`, `rev.com`, `creativecommons.org`), ASR fragments, and sponsor reads[^archive-data] |

# Domain Categories & Cross-Show Role

The 25 recurring domains cluster into four distinct functional roles across TWiT broadcasts:

1. **Security & Developer Utilities:** `grc.com` (9,893), `github.com` (97 across 11 shows), and `archive.org` (85 across 9 shows) anchor technical citations on [Security Now](../shows/sn.md), [FLOSS Weekly](../shows/floss.md), [Untitled Linux Show](../shows/uls.md), and [This Week in Tech](../shows/twit.md) whenever hosts direct listeners to source repositories, historical web snapshots, or free security utilities.[^archive-data]
2. **Platform & Streaming Portals:** `youtube.com` (537), `google.com` (518), `microsoft.com` (305), `amazon.com` (246), `x.com` (243), `twitter.com` (182), `apple.com` (149), and `twitch.tv` (73 across 11 shows) reflect both the platforms under discussion and live-streaming / social interaction channels.[^archive-data]
3. **Host Homepages, Books & Companion Podcasts:** `sixcolors.com` (267, [Jason Snell](../people/jason-snell.md)), `thurrott.com` (112, [Paul Thurrott](../people/paul-thurrott.md)), `leanpub.com` (108, Paul Thurrott's e-book platform), `runasradio.com` (30, [Richard Campbell](../people/richard-campbell.md)), `pylebooks.com` (29, [Rod Pyle](../people/rod-pyle.md)), `ihnatko.com` (28, [Andy Ihnatko](../people/andy-ihnatko.md)), `jeffjarvis.com` (26, [Jeff Jarvis](../people/jeff-jarvis.md)), and `rosemaryorchard.com` (24, [Rosemary Orchard](../people/rosemary-orchard.md)) appear primarily during panelist introductions and sign-off plugs.[^archive-data]
4. **Beat Journalism & Space Organizations:** `space.com` (354, [Tariq Malik](../people/tariq-malik.md)), `theregister.co` (57), `cnet.com` (51), `theverge.com` (27), `nss.org` (23, National Space Society), and `adastramagazine.com` (23, *Ad Astra*, edited by [Rod Pyle](../people/rod-pyle.md)) reflect direct URL citations on [This Week in Space](../shows/twis.md) and weekly news shows.[^archive-data]

# Top Non-Sponsor External Domains

| Domain | Official All-Time (Shows / 17) | Official 2025–2026 (Shows / 13) | YouTube Backfill (28 eps) |
|---|---|---|---|
| `grc.com` | 9,893 (3) | 230 (2) | 2 |
| `youtube.com` | 537 (13) | 59 (8) | 49 |
| `google.com` | 518 (12) | 21 (6) | 2 |
| `space.com` | 354 (8) | 251 (2) | 0 |
| `microsoft.com` | 305 (7) | 12 (4) | 1 |
| `sixcolors.com` | 267 (5) | 123 (3) | 0 |
| `amazon.com` | 246 (9) | 10 (6) | 2 |
| `x.com` | 243 (8) | 170 (6) | 1 |
| `twitter.com` | 182 (9) | 5 (2) | 5 |
| `apple.com` | 149 (9) | 23 (7) | 0 |
| `thurrott.com` | 112 (2) | 14 (1) | 0 |
| `leanpub.com` | 108 (1) | 43 (1) | 0 |
| `github.com` | 97 (11) | 16 (5) | 0 |
| `archive.org` | 85 (9) | 25 (5) | 3 |
| `twitch.tv` | 73 (11) | 19 (9) | 4 |
| `theregister.co` | 57 (2) | 0 (0) | 0 |
| `cnet.com` | 51 (4) | 15 (2) | 0 |
| `runasradio.com` | 30 (1) | 24 (1) | 0 |
| `pylebooks.com` | 29 (1) | 28 (1) | 0 |
| `ihnatko.com` | 28 (2) | 18 (1) | 0 |
| `theverge.com` | 27 (3) | 21 (2) | 0 |
| `jeffjarvis.com` | 26 (1) | 26 (1) | 0 |
| `rosemaryorchard.com` | 24 (2) | 15 (2) | 0 |
| `nss.org` | 23 (2) | 21 (2) | 0 |
| `adastramagazine.com` | 23 (1) | 21 (1) | 0 |

# Sponsor Filtering & Extraction Methodology

Podcast transcripts contain thousands of ad-read URLs and boilerplate transcription footers that would otherwise swamp editorial domain rankings. Accordingly, the extraction pipeline explicitly filters out:

- **Network self-links:** `twit.tv`, `twi.tv`.[^archive-data]
- **Transcription & license footers:** `creativecommons.org`, `temi.com`, `rev.com`.[^archive-data]
- **Recurring podcast sponsor domains:** `stamps.com`, `audible.com`, `ziprecruiter.com`, `melissa.com`, `cachefly.com`, `zscaler.com`, `threatlocker.com`, `helixsleep.com`, `spaceship.com`, `outsystems.com`, `joindeleteme.com`, and similar ad-read URLs, alongside automated speech-recognition (ASR) punctuation fragments.[^archive-data]

# See Also

- **Entities:** [GRC and Security Tools](../entities/grc-and-security-tools.md), [Apple](../entities/apple.md), [Microsoft](../entities/microsoft.md), [Google](../entities/google.md), [NASA and SpaceX](../entities/nasa-and-spacex.md), [Linux and FOSS Ecosystem](../entities/linux-and-foss.md).[^archive-data]
- **Key Voices:** [Steve Gibson](../people/steve-gibson.md), [Jason Snell](../people/jason-snell.md), [Paul Thurrott](../people/paul-thurrott.md), [Tariq Malik](../people/tariq-malik.md), [Rod Pyle](../people/rod-pyle.md), [Jeff Jarvis](../people/jeff-jarvis.md), [Richard Campbell](../people/richard-campbell.md), [Andy Ihnatko](../people/andy-ihnatko.md), [Rosemary Orchard](../people/rosemary-orchard.md).[^archive-data]
- **Companion References:** [Publications and Newsletters](../references/publications-and-newsletters.md), [Notable People](../references/notable-people.md), [Organizations and Tools](../references/organizations-and-tools.md)

[^archive-data]: Processed official TWiT transcript Markdown chunks (577 files, 3,350 episodes)
[^yt-data]: YouTube caption backfill transcripts (28 files, unattributed)
[^dataset-doc]: TWiT Transcript Archive dataset specification
