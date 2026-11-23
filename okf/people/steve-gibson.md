---
type: person
title: "Steve Gibson"
description: "Security Researcher & Co-Host of Security Now; appears as a speaker in 1,150 official episodes across 5 shows (2005–2026)."
tags: [person, host, security, grc]
generated: { by: "antigravity/gemini-4-neon-medium", at: "2026-11-23T21:40:00Z" }
sources:
  - id: archive-data
    resource: "local archive data/*_Transcripts_*.md"
    title: "Processed official TWiT transcript Markdown chunks (577 files, 3,350 episodes)"
  - id: dataset-doc
    resource: /datasets/twit-transcript-archive.md
    title: "TWiT Transcript Archive dataset specification"
---

Steve Gibson is a veteran computer security researcher, assembly-language programmer, founder of Gibson Research Corporation (`grc.com`), and co-host of [Security Now](../shows/sn.md) alongside [Leo Laporte](leo-laporte.md). Backed by GRC.com's complete historical transcript archive, Gibson's catalog is the longest-running continuous single-show record in the dataset, spanning from 2005 through 2026.[^archive-data][^dataset-doc]

Gibson's weekly deep dives form the technical backbone of the archive's [Cybersecurity and Privacy](../topics/cybersecurity-and-privacy.md) coverage, translating low-level networking protocols, cryptographic primitives, browser internals, and zero-day CVEs into structured weekly briefings for IT professionals and security-minded listeners.[^archive-data]

# Quick Facts

| Attribute | Value |
|---|---|
| **Role** | Security Researcher & Co-Host of Security Now |
| **Archive Span** | 2005–2026 |
| **Official Speaker Episodes** | 1,150 across 5 shows |
| **Spoken Body Mentions** | 6,732 across 17 shows |
| **Attributed Speaker Turns** | 133,126 turns (11,636,675 spoken words) |
| **Associated Publications / Domains** | GRC.com, Security Now (`grc.com`) |

# Presence & Trajectory Across the TWiT Archive

Across the 3,350 official attributed episodes in the [TWiT Transcript Archive](../datasets/twit-transcript-archive.md), Steve Gibson logs **1,150 speaker episodes** across 5 shows (133,126 attributed turns totaling 11,636,675 spoken words) and **6,732 spoken body mentions** across 17 shows.[^archive-data] Activity spans **2005–2026**, with 492 speaker episodes in 2005–2020, 45 in 2021–2024, and 41 in 2025–2026 (plus 572 in undated legacy transcripts). Note that unattributed YouTube caption backfills in `data_youtube/` are deliberately excluded from speaker-attributed counts.[^archive-data]

## Breakdown by Show

| Show | Episode Appearances | Spoken Body Mentions |
|---|---|---|
| [Security Now](../shows/sn.md) (`SN`) | 1,094 | 6,092 |
| [This Week in Tech](../shows/twit.md) (`TWIT`) | 50 | 186 |
| [Macbreak Weekly](../shows/mbw.md) (`MBW`) | 3 | 85 |
| [Windows Weekly](../shows/ww.md) (`WW`) | 2 | 112 |
| [Before You Buy](../shows/byb.md) (`BYB`) | 1 | 10 |

## Activity by Era

| Period | Speaker Episodes |
|---|---|
| 2005–2020 | 492 |
| 2021 | 17 |
| 2022 | 11 |
| 2023 | 8 |
| 2024 | 9 |
| 2025 | 13 |
| 2026 | 28 |
| Undated (year 0) | 572 |

# Editorial Perspective & Signature Themes

Gibson's editorial stance is rooted in first-principles engineering, protocol minimalism, and verifiable trust. He consistently advocates for clean cryptographic design—championing WireGuard over legacy VPN stacks, passkeys and password managers over reused credentials, and transparent open-source audits over security through obscurity. While skeptical of bloated enterprise software and opaque cloud telemetry, his 2024–2026 episodes reflect notable enthusiasm for large language models as personal research and productivity assistants, paired with careful scrutiny of AI-enabled attack surfaces and software supply-chain risks.[^archive-data]

- **Topics:** [Cybersecurity and Privacy](../topics/cybersecurity-and-privacy.md) (32,621 co-occurring mentions), [Windows and Microsoft](../topics/windows-and-microsoft.md) (21,538 co-occurring mentions), [Android and Mobile](../topics/android-and-mobile.md) (19,968 co-occurring mentions), [Apple Ecosystem](../topics/apple-ecosystem.md) (16,064 co-occurring mentions), [Linux and Open Source](../topics/linux-and-open-source.md) (7,946 co-occurring mentions).[^archive-data]
- **Entities:** [GRC and Security Tools](../entities/grc-and-security-tools.md) (26,227 co-occurring mentions), [Microsoft](../entities/microsoft.md) (15,727 co-occurring mentions), [Google](../entities/google.md) (15,328 co-occurring mentions), [Apple](../entities/apple.md) (11,314 co-occurring mentions), [Mozilla and the Open Web](../entities/mozilla-and-open-web.md) (7,268 co-occurring mentions).[^archive-data]

## Recurring Points of View & Verbatim Quotes

All quotes below are extracted verbatim from speaker-attributed turns in the 3,350 official Markdown transcripts (excluding sponsor reads and unattributed YouTube captions).[^archive-data]

### [AI and LLMs](../viewpoints/ai-and-llms.md)

On **AI and LLMs**, Steve Gibson's attributed on-air remarks reflect recurring analytical priorities across multiple episodes:[^archive-data]

> "I should note that I already have everything I need, thanks to today's ChatGPT 4.0. And it has changed my life for the better." — [Security Now](../shows/sn.md) #1001, Undated[^archive-data]

> "I think that the most accurate and succinct way of describing what we're witnessing is that it is astonishing to see the degree to which a neural network using large language modeling, as exemplified by ChatGPT, is able to simulate intelligence. And I think that is the key concept to hold onto." — [Security Now](../shows/sn.md) #911, Undated[^archive-data]

> "So I think it's a combination of the effects of this LLM model temperature, different model training in detail, and difference in the specific prompting that the differing models are given. In other words, the use of LLMs for software vulnerability discovery is still very new, and there are still a great many variables that can affect its results." — [Security Now](../shows/sn.md) #1084, Undated[^archive-data]

### [Windows and Microsoft Copilot](../viewpoints/windows-and-microsoft-copilot.md)

On **Windows and Microsoft Copilot**, Steve Gibson's attributed on-air remarks reflect recurring analytical priorities across multiple episodes:[^archive-data]

> "So when I'm downloading actual content from somewhere, like I did last week, the Windows 11 24H2 ISO, which is 5.6GB, while it was downloading, I was able just to glance up at the screen and see what my actual bandwidth being delivered to me from Microsoft was. So, you know, it's nice to have that." — [Security Now](../shows/sn.md) #1024, 2025-05-12[^archive-data]

> "The researcher said: 'I think it will take a while even for MSRC [Microsoft Security Research] to find the real root cause of the issue." I don't think so, but that's what he said." — [Security Now](../shows/sn.md) #1079, 2026-05-22[^archive-data]

> "Microsoft's perpetually security-challenged Remote Desktop Protocol usage, based on the presence of available ports - that is, 3389, publicly present on the Internet - has jumped 41%. And popular VPN port appearances have gone up by a third, 33%." — [Security Now](../shows/sn.md) #760, 2019-02-01[^archive-data]

### [Cybersecurity and Privacy](../viewpoints/cybersecurity-and-privacy.md)

On **Cybersecurity and Privacy**, Steve Gibson's attributed on-air remarks reflect recurring analytical priorities across multiple episodes:[^archive-data]

> "The researcher said: 'I think it will take a while even for MSRC [Microsoft Security Research] to find the real root cause of the issue." I don't think so, but that's what he said." — [Security Now](../shows/sn.md) #1079, 2026-05-22[^archive-data]

> "Something called Tailscale, T-A-I-L-S-C-A-L-E. As we know, WireGuard is widely, and I think appropriately and accurately, regarded as the logical and overdue successor to the venerable OpenVPN, and even to some degree IPSec, inasmuch as it can replace them both." — [Security Now](../shows/sn.md) #830, Undated[^archive-data]

> "I think that a better way would be to notify the public on day zero that there are vulnerabilities and what is the impact, to notify the public and the vendor together, and not to disclose the actual technical details ever unless it's already fixed; to put the full public pressure on the vendor from the get-go, but to never put customers at risk." — [Security Now](../shows/sn.md) #655, 2018-03-20[^archive-data]

### [Linux and Open Source](../viewpoints/linux-and-open-source.md)

On **Linux and Open Source**, Steve Gibson's attributed on-air remarks reflect recurring analytical priorities across multiple episodes:[^archive-data]

> "He describes himself as - I think this was in his little short bio on GitHub: "Random infosec guy. Rainbow teamer." — [Security Now](../shows/sn.md) #830, Undated[^archive-data]

> "So the news that I'm excited about - and Leo, I know you are excited about it - it was by far the most tweeted bit of news I was receiving last week is the news that Threema has decided to go open source, and also to welcome a new partner. They announced it, I think it was last Thursday." — [Security Now](../shows/sn.md) #783, Undated[^archive-data]

> "And then he tweeted to me the link to "The Horror of LessPass" on the TWiT netcast network. And he sent me a link to the GitHub thread where he's completely explained his position." — [Security Now](../shows/sn.md) #587, Undated[^archive-data]

# Frequently Cited Publications, Domains & Collaborators

- **Publications & Domains:** GRC.com, Security Now (`grc.com`) — see [Publications and Newsletters](../references/publications-and-newsletters.md) and [Recurring External Domains](../references/recurring-domains.md).[^archive-data]
- **Most Frequent Archive Collaborators / Co-Appearing Hosts:** [Leo Laporte](leo-laporte.md) (1,077 shared episodes), [Jason Howell](jason-howell.md) (52 shared episodes), [Paul Thurrott](paul-thurrott.md) (11 shared episodes), [Mikah Sargent](mikah-sargent.md) (10 shared episodes), [Jason Snell](jason-snell.md) (7 shared episodes), [Jeff Jarvis](jeff-jarvis.md) (6 shared episodes).[^archive-data]

## See Also

- [People Index](index.md) — All 20 profiled TWiT hosts, panelists, journalists, and researchers.
- [Notable People Reference](../references/notable-people.md) — Network-wide ranking of hosts and cited experts.
- **Related Viewpoints:** [AI and LLMs](../viewpoints/ai-and-llms.md), [Windows and Microsoft Copilot](../viewpoints/windows-and-microsoft-copilot.md), [Cybersecurity and Privacy](../viewpoints/cybersecurity-and-privacy.md), [Linux and Open Source](../viewpoints/linux-and-open-source.md).
- [TWiT Transcript Archive](../datasets/twit-transcript-archive.md) — Full corpus specification and attribution methodology.

[^archive-data]: Processed official TWiT transcript Markdown chunks (577 files, 3,350 episodes)
[^dataset-doc]: TWiT Transcript Archive dataset specification
