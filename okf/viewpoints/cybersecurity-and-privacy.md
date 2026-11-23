---
type: viewpoint
title: "Cybersecurity and Privacy"
description: "Cross-host viewpoints and verbatim quotes on encryption, passkeys, ransomware, zero-day vulnerabilities, password managers, surveillance, and digital privacy."
tags: [viewpoint, cybersecurity, privacy, encryption, passkeys, quotes]
generated: { by: "antigravity/gemini-4-neon-medium", at: "2026-11-23T21:40:00Z" }
sources:
  - id: archive-data
    resource: "local archive data/*_Transcripts_*.md"
    title: "Processed official TWiT transcript Markdown chunks (577 files, 3,350 episodes)"
  - id: dataset-doc
    resource: /datasets/twit-transcript-archive.md
    title: "TWiT Transcript Archive dataset specification"
---

Cybersecurity and personal privacy form the longest-running technical thread in the TWiT archive, anchored by more than 1,090 episodes of [Security Now](../shows/sn.md) and reinforced weekly across [This Week in Tech](../shows/twit.md), [Untitled Linux Show](../shows/uls.md), and [Windows Weekly](../shows/ww.md). Over two decades, the network's focus has evolved from consumer firewalls and Wi-Fi encryption to passkeys, password managers, WireGuard/Tailscale mesh networking, ransomware economics, software supply-chain compromises, and post-quantum cryptography.[^archive-data][^dataset-doc]

This article gathers verbatim attributed perspectives from TWiT's security specialists alongside cited authorities including [Bruce Schneier](../people/bruce-schneier.md) and [Brian Krebs](../people/brian-krebs.md).[^archive-data]

# Quick Facts

| Attribute | Value |
|---|---|
| **Attributed Opinion Turns Mined** | 4,810 turns (903 in 2025–2026) |
| **Primary Shows** | [Security Now](../shows/sn.md), [This Week in Tech](../shows/twit.md), [Untitled Linux Show](../shows/uls.md), [Windows Weekly](../shows/ww.md), [Macbreak Weekly](../shows/mbw.md) |
| **Related Topics** | [Cybersecurity and Privacy](../topics/cybersecurity-and-privacy.md) |
| **Related Entities** | [GRC and Security Tools](../entities/grc-and-security-tools.md), [EFF and Digital Rights](../entities/eff-and-digital-rights.md), [Mozilla and the Open Web](../entities/mozilla-and-open-web.md) |

# Key Fault Lines & Consensus Areas

- **Usability vs. maximalist threat modeling:** Consumer-oriented hosts like [Leo Laporte](../people/leo-laporte.md) and [Mikah Sargent](../people/mikah-sargent.md) emphasize friction-free defaults (passkeys, mainstream password managers, automatic OS updates), while [Steve Gibson](../people/steve-gibson.md) and [Jonathan Bennett](../people/jonathan-bennett.md) examine low-level protocol flaws, kernel attack surfaces, and self-hosted alternatives.
- **Corporate accountability vs. individual hygiene:** Journalists like [Paris Martineau](../people/paris-martineau.md) and [Cory Doctorow](../people/cory-doctorow.md) argue that data-broker surveillance and weak breach liability require legislative remedies rather than pushing all burden onto consumers.
- **Consensus area:** Universal agreement against government encryption backdoors, strong endorsement of open-standard cryptography (WireGuard, Signal, FIDO2/Passkeys), and skepticism of opaque closed-source security claims.[^archive-data]

## Attributed Opinion Volume by Period

| Period | Attributed Opinion Turns |
|---|---|
| Pre-2020 | 2,454 |
| 2020 | 92 |
| 2021 | 124 |
| 2022 | 371 |
| 2023 | 407 |
| 2024 | 459 |
| 2025 | 476 |
| 2026 | 427 |

# Perspectives by Host & Contributor

Every blockquote below is extracted verbatim from speaker-attributed turns in the 3,350 official Markdown transcripts (excluding sponsor reads and unattributed YouTube captions).[^archive-data]

## [Alex Lindsay](../people/alex-lindsay.md)

**Alex Lindsay** (Media Production Technologist & Macbreak Weekly Panelist) brings a distinct recurring lens to Cybersecurity and Privacy discussions across the archive:[^archive-data]

> "The, the, the issue is, is going to keep on coming back to content, but I think that one of the things that Apple has that Meta doesn't have is, I think that Apple is, they keep on spending resources on privacy and trust, and I think that that foils Meta in a way that Meta can't really turn the corner on, which is that you're talking about." — [Macbreak Weekly](../shows/mbw.md) #941, 2024-10-02, TS:1:25:54[^archive-data]

> "They did you could do hangouts between two glass and they turned that off, like this security issue. So, but the, but the, um, uh, but the." — [Macbreak Weekly](../shows/mbw.md) #958, 2025-02-05, TS:1:56:54[^archive-data]

## [Steve Gibson](../people/steve-gibson.md)

**Steve Gibson** (Security Researcher & Co-Host of Security Now) brings a distinct recurring lens to Cybersecurity and Privacy discussions across the archive:[^archive-data]

> "The researcher said: 'I think it will take a while even for MSRC [Microsoft Security Research] to find the real root cause of the issue." I don't think so, but that's what he said." — [Security Now](../shows/sn.md) #1079, 2026-05-22[^archive-data]

> "Something called Tailscale, T-A-I-L-S-C-A-L-E. As we know, WireGuard is widely, and I think appropriately and accurately, regarded as the logical and overdue successor to the venerable OpenVPN, and even to some degree IPSec, inasmuch as it can replace them both." — [Security Now](../shows/sn.md) #830, Undated[^archive-data]

## [Jason Snell](../people/jason-snell.md)

**Jason Snell** (Founder of Six Colors & Macbreak Weekly Panelist) brings a distinct recurring lens to Cybersecurity and Privacy discussions across the archive:[^archive-data]

> "I think that there's already a better model that allows that level of security and safety and then lets you gradually step out of it. And guess who built that model?" — [Macbreak Weekly](../shows/mbw.md) #949, 2024-11-27, TS:1:33:51[^archive-data]

> "I, my favorite line in the entire piece is that thing about the flexible, elastic garment for as a shield for security Only, because I mean, this is where trouble again, because I think that apple I don't ascribe, I don't believe that, uh, apple doesn't believe in privacy." — [Macbreak Weekly](../shows/mbw.md) #914, 2024-03-26, TS:0:37:08[^archive-data]

## [Leo Laporte](../people/leo-laporte.md)

**Leo Laporte** (TWiT Network Founder & Host) brings a distinct recurring lens to Cybersecurity and Privacy discussions across the archive:[^archive-data]

> "Got to love the Bitwarden, the only password manager I recommend these days. It's offering a cost-effective solution that can dramatically improve your chances of staying safe online and, by the way, by itself, bitwarden does everything you need." — [This Week in Tech](../shows/twit.md) #988, 2024-07-14, TS:01:32:01[^archive-data]

> "This is an unacceptable security violation and visitors will have to check their Apple devices at the door while they be stored in a Faraday cage. He's sounding nuts." — [Macbreak Weekly](../shows/mbw.md) #953, 2024-12-22, TS:2:15:48[^archive-data]

## [Paul Thurrott](../people/paul-thurrott.md)

**Paul Thurrott** (Tech Journalist & Co-Host of Windows Weekly / Hands-On Windows) brings a distinct recurring lens to Cybersecurity and Privacy discussions across the archive:[^archive-data]

> "I believe that 1Password is probably the most complete in that way, if you will, protonpass and Dashlane and Bitwarden are pretty close. If they don't have all five, it's four of the five." — [Hands-On Windows](../shows/how.md) #103, 2024-08-15, TS:0:00:00[^archive-data]

> "You know it's like yeah, it's a little more sophisticated than that and and I, I, I think people are not giving it it its due and I think when you put kind of invented privacy concerns or security concerns in front of the conversation, you can't see the forest for the trees, that there's something kind of really cool happening here." — [Windows Weekly](../shows/ww.md) #898, 2024-09-11, TS:0:58:45[^archive-data]

## [Mikah Sargent](../people/mikah-sargent.md)

**Mikah Sargent** (TWiT Host (iOS Today, Hands-On Tech, Hands-On Apple, Tech News Weekly)) brings a distinct recurring lens to Cybersecurity and Privacy discussions across the archive:[^archive-data]

> "So I think that that answers the question of, or answers the problem that some privacy advocates had with it, answers the problem that some privacy advocates had with it. But ultimately I do wonder what the size of this market actually is and how many people are even aware that this is a possibility." — [Tech News Weekly](../shows/tnw.md) #396, 2025-07-18, TS:0:25:43[^archive-data]

> "That's the way that I recommend going for now, because of the fact that they are cross-platform, so you're not dealing with the issue of well, it's on my phone, saved in my iCloud, but now if I have to log in on a work computer and it's a Windows machine, do I have access to that passkey? That's why we're all touting the third-party password manager." — [Tech News Weekly](../shows/tnw.md) #368, 2025-01-02, TS:1:01:35[^archive-data]

## [Andy Ihnatko](../people/andy-ihnatko.md)

**Andy Ihnatko** (Technology Columnist & Macbreak Weekly Panelist) brings a distinct recurring lens to Cybersecurity and Privacy discussions across the archive:[^archive-data]

> "However, that doesn't come at no cost to how well their products work, and so I think eternally and certainly for the foreseeable future, there's going to always be that question of, if we compromise privacy a little bit and not so much that there is anything we can point to that's tangible that people are losing by giving up this much privacy and give the…" — [Macbreak Weekly](../shows/mbw.md) #968, 2025-04-16, TS:0:41:54[^archive-data]

> "I think that just like an iPhone has a signature design, any service that they provide is going to have a signature set of understandings around it which is privacy and security. That Apple does not know what you're doing on this device and does not care what you're doing on what you're doing on this device." — [Macbreak Weekly](../shows/mbw.md) #1001, 2025-12-04, TS:00:23:43[^archive-data]

# Cited External Voices & Analysts

TWiT hosts frequently cite external beat journalists, cryptographers, and industry analysts to anchor debates on **Cybersecurity and Privacy**.[^archive-data]

### [Bruce Schneier](../people/bruce-schneier.md)

**Bruce Schneier** (Cited Cryptographer, Security Technologist & Author) is regularly invoked by TWiT panelists to ground Cybersecurity and Privacy reporting and analysis:[^archive-data]

> "But when we recall Bruce Schneier's reminder - "Attacks never get weaker, they only ever get stronger" - you know, it seems like what might be a curiosity today could have the tendency to mature over time. So how to fix this?" — Cited by Steve, [Security Now](../shows/sn.md) #1051, 2026-11-17[^archive-data]

> "And as we're going to find out, that determination and Bruce Schneier's brilliantly labeled "Genie effect," it's what's going on with our AI. And I think if I had a single reason to be concerned, and everyone's been listening to me about AI since the beginning, I've never really been concerned." — Cited by Steve, [Security Now](../shows/sn.md) #1091, Undated[^archive-data]

### [Brian Krebs](../people/brian-krebs.md)

**Brian Krebs** (Cited Investigative Cybersecurity Journalist (Krebs on Security)) is regularly invoked by TWiT panelists to ground Cybersecurity and Privacy reporting and analysis:[^archive-data]

> "Brian Krebs, writing about this month's consequences for his Krebs on Security blog, wrote, Microsoft Corp. today issued updates to plug at least 974 security holes in its Windows operating systems and other software." — Cited by Steve Gibson, [Security Now](../shows/sn.md) #1096, 2026-09-15, TS:00:10:22[^archive-data]

> "And I love Brian Krebs. The title of his blog post about this was "Java Update: Patch It or Pitch It." And so he said: "Oracle today released a security update for its Java platform that addresses at least 20 vulnerabilities in the software." — Cited by Steve, [Security Now](../shows/sn.md) #465, Undated[^archive-data]

### [Cory Doctorow](../people/cory-doctorow.md)

**Cory Doctorow** (Author, EFF Special Advisor & Frequent TWiT Guest) is regularly invoked by TWiT panelists to ground Cybersecurity and Privacy reporting and analysis:[^archive-data]

> "We, we, we Torontonians, we stick together, so we're like, we're like this. So yeah, the, the, the I guess the, the, I think that the security trade off is a bad one. And I think the companies," — [This Week in Tech](../shows/twit.md) #873, 2022-05-02, TS:01:22:06[^archive-data]

> "And sometimes that's appropriate. But I think with both privacy and with the access act a private right of action makes sense." — [This Week in Tech](../shows/twit.md) #895, 2022-10-03, TS:00:23:42[^archive-data]

### [Mark Gurman](../people/mark-gurman.md)

**Mark Gurman** (Cited Journalist (Bloomberg Apple Reporter)) is regularly invoked by TWiT panelists to ground Cybersecurity and Privacy reporting and analysis:[^archive-data]

> "I might have to write him and send him mine On to the Mark Gurman continued with the Mark Gurman segment that we really went far afield on that one. He did say, which will be a little disappointment to some people, that there will be new iPads, but there are a number of things who that will not come out." — Cited by Leo Laporte, [Macbreak Weekly](../shows/mbw.md) #955, 2025-01-15, TS:1:17:55[^archive-data]

> "time zones for your other offices, so there's a lot of variety and it's all running off something called nano time kit and Mark Gurman from 9to5 Mac was reporting that they were already considering the 3 rd party complications because that framework, like most of Apple's frameworks can be extended. So it's going to be really interesting to see." — Cited by Rene, [Macbreak Weekly](../shows/mbw.md) #455, 2015-06-07[^archive-data]

## See Also

- [Viewpoints Index](index.md) — All 7 cross-host topical debate articles.
- [People Index](../people/index.md) — Full archive biographies for all 20 hosts and cited experts.
- **Related Topics:** [Cybersecurity and Privacy](../topics/cybersecurity-and-privacy.md).
- **Related Entities:** [GRC and Security Tools](../entities/grc-and-security-tools.md), [EFF and Digital Rights](../entities/eff-and-digital-rights.md), [Mozilla and the Open Web](../entities/mozilla-and-open-web.md).

[^archive-data]: Processed official TWiT transcript Markdown chunks (577 files, 3,350 episodes)
[^dataset-doc]: TWiT Transcript Archive dataset specification
