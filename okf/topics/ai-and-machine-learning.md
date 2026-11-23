---
type: topic
title: "AI and Machine Learning"
description: "Fastest-growing topic cluster across the TWiT archive, led by LLMs, OpenAI, Anthropic Claude, Microsoft Copilot, AI agents, and coding assistants."
tags: [topic, ai, llm, openai, anthropic, copilot, agents]
generated: { by: "antigravity/gemini-4-neon-medium", at: "2026-11-23T22:55:00Z" }
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
  - id: grc-sn
    resource: https://www.grc.com/securitynow.htm
    title: "GRC.com Security Now transcript archive"
---

**AI and Machine Learning** is the fastest-growing topic cluster in the [TWiT Transcript Archive](../datasets/twit-transcript-archive.md), spanning 3,350 official episodes (577 processed Markdown chunks) alongside 28 unattributed YouTube caption backfills.[^archive-data][^yt-data][^dataset-doc] Broad artificial intelligence references reach 55,843 mentions across 16 of 17 official shows all-time, with 30,063 of those mentions concentrated in the 2025–2026 window across all 13 active shows.[^archive-data] What began before 2020 as an occasional background subject in general technology and security discussions transformed after 2022 into an all-encompassing editorial beat spanning large language models (LLMs), autonomous agents, AI-assisted software development, local model inference, enterprise productivity suites, and AI security risks.[^archive-data]

The topic's center of gravity spans both dedicated AI commentary and network-wide cross-pollination. Primary shows driving this cluster include [Intelligent Machines](../shows/im.md), [This Week in Tech](../shows/twit.md), [Windows Weekly](../shows/ww.md), [Tech News Weekly](../shows/tnw.md), and [This Week in Google](../shows/twig.md), while [Security Now](../shows/sn.md) contributes several of the highest-signal individual episodes in the entire corpus through deep technical analyses of LLM jailbreaking, token-stream vulnerabilities, and maliciously trained models.[^archive-data] Rather than remaining siloed inside a single program, AI coverage permeates operating system shows, consumer hardware reviews, and legal policy roundtables, making it the primary connective tissue of the 2025–2026 TWiT schedule.[^archive-data]

Editorial debates recorded across the archive reflect rapid shifts in both capability and competitive positioning. Early generative AI episodes focused on novelty, image and video synthesis, and broad disruption narratives, whereas 2025–2026 transcripts document intense rivalry between [OpenAI](../entities/openai.md) and [Anthropic](../entities/anthropic.md), the mainstream adoption of coding assistants and remote agent sessions, local open-weight models such as DeepSeek, and growing concern over agentic security failures and defense-sector contracts.[^archive-data] For verbatim cross-host perspectives on these debates, see [AI and LLMs](../viewpoints/ai-and-llms.md).[^archive-data]

| Attribute | Value |
|---|---|
| **Type** | Topic (`okf/topics`) |
| **Primary Shows** | [Intelligent Machines](../shows/im.md), [This Week in Tech](../shows/twit.md), [Windows Weekly](../shows/ww.md), [Tech News Weekly](../shows/tnw.md), [This Week in Google](../shows/twig.md), [Security Now](../shows/sn.md) |
| **Top Subtopic** | AI / Artificial Intelligence (55,843 all-time; 30,063 in 2025–2026) |
| **2025–2026 Momentum** | 13,959 topic-level keyword mentions (7,213 in 2025; 6,746 in 2026); 30,063 broad AI mentions across 13/13 active shows |
| **Peak Year** | 2025 (7,213 topic keyword mentions; 2026 closely trailing at 6,746) |
| **YouTube Backfill Hits** | 23 topic-level hits (88 broad AI, 12 Grok/xAI, 10 Anthropic/Claude, 6 OpenAI/ChatGPT) across 28 episodes |
| **Related Viewpoint** | [AI and LLMs](../viewpoints/ai-and-llms.md) |

# Historical Arc & Year-by-Year Trajectory

Across the archive's longitudinal timeline, AI and Machine Learning exhibits the sharpest hockey-stick inflection of any tracked topic cluster.[^archive-data] During the entire pre-2020 official archive—covering more than a decade of legacy transcripts—topic-level keyword mentions totaled just 188, followed by 0 dated hits in 2020 and 19 in 2021.[^archive-data] Even in 2022, when early generative tools began entering public view, dated official mentions reached only 81, reflecting both sparse archive transcript coverage in 2020–2021 and the pre-mainstream status of consumer LLMs.[^archive-data][^dataset-doc]

The structural breakout arrived in 2023 and accelerated dramatically through 2024. Topic keyword mentions jumped more than eighteen-fold from 81 in 2022 to 1,477 in 2023, then more than doubled again to 3,121 in 2024 as ChatGPT, [Microsoft](../entities/microsoft.md) Copilot, [Google](../entities/google.md) Gemini, and early Apple Intelligence announcements reshaped weekly show rundowns.[^archive-data] During this 2023–2024 transition, hosts moved from explaining foundational transformer concepts and prompt experimentation to tracking enterprise rollouts, copyright litigation, and model benchmarks.[^archive-data]

In 2025–2026, AI coverage reached network-wide saturation. Mentions surged to a peak of 7,213 in 2025 and sustained nearly identical intensity in 2026 with 6,746 mentions—meaning 2025 and 2026 together account for the overwhelming majority of dated topic-level mentions in the archive.[^archive-data] Notably, this surge coincided with the evolution of [This Week in Google](../shows/twig.md) into [Intelligent Machines](../shows/im.md) and the emergence of [Security Now](../shows/sn.md) episodes devoted almost entirely to AI threat modeling.[^archive-data] The 28 unattributed YouTube backfill episodes contribute an additional 23 topic-level mentions, supplementing gaps in the official feed.[^yt-data]

| Period | Topic Keyword Mentions |
|---|---|
| Pre-2020 (official) | 188 |
| 2020 | 0 |
| 2021 | 19 |
| 2022 | 81 |
| 2023 | 1,477 |
| 2024 | 3,121 |
| 2025 | 7,213 |
| 2026 | 6,746 |
| YouTube Caption Backfill (`data_youtube/`) | 23 |

# Subtopic Landscape & Thematic Analysis

Disaggregating the subtopic mention table reveals how the AI conversation diversified from a single-vendor story into a multi-front ecosystem war.[^archive-data] Beyond the umbrella `AI / Artificial Intelligence` term (55,843 all-time; 30,063 in 2025–2026), [OpenAI](../entities/openai.md) / ChatGPT leads all-time vendor mentions at 5,936 across 15 shows, followed closely by [Anthropic](../entities/anthropic.md) / Claude at 4,865 across 14 shows and [Microsoft](../entities/microsoft.md) Copilot at 4,047 across 11 shows.[^archive-data] However, the 2025–2026 window reveals a striking momentum shift: Anthropic / Claude recorded 3,838 mentions across 12 shows in 2025–2026—surpassing OpenAI / ChatGPT's 3,647 mentions in the same period—reflecting intense host engagement with Claude Code, remote sessions, and Anthropic's rapid model cadence.[^archive-data]

A second major tier comprises competing model ecosystems and platform integrations. [Google](../entities/google.md) Gemini, NotebookLM, and DeepSeek together account for 3,025 all-time mentions (1,903 in 2025–2026 across 12 shows), capturing both Google's consumer AI push and the shockwave triggered by local-capable open-weight models like DeepSeek.[^archive-data] Apple Intelligence accounts for 1,196 mentions across 12 shows (610 in 2025–2026), while Perplexity AI logs 1,188 mentions across 10 shows (897 in 2025–2026) and Grok / xAI logs 661 all-time mentions (570 in 2025–2026, plus 12 hits in the YouTube backfill—the highest single-vendor backfill count after general AI).[^archive-data][^yt-data]

Equally telling is the explosive rise of workflow-oriented subtopics in 2025–2026. `Large Language Models (LLMs)` stands at 3,315 all-time mentions (1,703 in 2025–2026), while `AI Agents / Agentic AI / MCP` jumped to 1,709 all-time mentions with 1,389 occurring in 2025–2026 across all 13 active shows.[^archive-data] Similarly, `Vibe Coding / AI Coding` recorded 964 all-time mentions, of which 808 appeared in 2025–2026 across 9 shows.[^archive-data] Across these transcripts, editorial fault lines center on three recurring tensions: hands-on developer productivity versus unverified code quality, autonomous agent convenience versus catastrophic financial or system-level mishaps, and frontier lab governance versus commercial and defense pressures.[^archive-data]

| Subtopic | Official All-Time (Shows / 17) | Official 2025–2026 (Shows / 13) | YouTube Backfill (28 eps) |
|---|---|---|---|
| AI / Artificial Intelligence | 55,843 (16) | 30,063 (13) | 88 |
| OpenAI / ChatGPT | 5,936 (15) | 3,647 (13) | 6 |
| Microsoft Copilot | 4,047 (11) | 2,464 (10) | 0 |
| Anthropic / Claude | 4,865 (14) | 3,838 (12) | 10 |
| Large Language Models (LLMs) | 3,315 (13) | 1,703 (12) | 2 |
| AI Agents / Agentic AI / MCP | 1,709 (13) | 1,389 (13) | 2 |
| Vibe Coding / AI Coding | 964 (11) | 808 (9) | 0 |
| Perplexity AI | 1,188 (10) | 897 (9) | 0 |
| Apple Intelligence | 1,196 (12) | 610 (10) | 0 |
| Google Gemini / NotebookLM / DeepSeek | 3,025 (13) | 1,903 (12) | 0 |
| Grok / xAI | 661 (12) | 570 (9) | 12 |

# Cross-Show Editorial Coverage & Key Voices

Different programs across the TWiT network approach AI and Machine Learning through distinct editorial lenses, creating a layered record of industry reaction.[^archive-data] [Intelligent Machines](../shows/im.md)—hosted by [Leo Laporte](../people/leo-laporte.md), [Jeff Jarvis](../people/jeff-jarvis.md), and [Paris Martineau](../people/paris-martineau.md), with guest hosts such as Jason Hiner and reporters including Emily Forlini—serves as the network's dedicated weekly forum for AI product launches, Silicon Valley talent battles, media impact, and agentic mishaps.[^archive-data] Laporte frequently brings hands-on experimentation to the table, testing local hardware and remote Claude Code sessions on his Framework desktop, while Martineau supplies investigative skepticism about hype and real-world agent failures, and Jarvis frames developments through journalism, institutional power, and public-sphere norms.[^archive-data]

By contrast, [Security Now](../shows/sn.md) approaches AI from a systems-architecture and adversarial-security perspective. [Steve Gibson](../people/steve-gibson.md) and Laporte dissect research papers on prompt injection, jailbreaking, maliciously trained models, and why the underlying token-stream design of LLMs resists traditional deterministic security boundaries—even while Gibson himself notes practical day-to-day utility in querying Claude and running local models enabled by DeepSeek.[^archive-data] Meanwhile, [Windows Weekly](../shows/ww.md)—anchored by [Paul Thurrott](../people/paul-thurrott.md) and [Richard Campbell](../people/richard-campbell.md)—tracks Microsoft Copilot's enterprise licensing, Windows integration, and hardware ties to [NVIDIA](../entities/nvidia.md) and NPU-equipped PCs, while [This Week in Tech](../shows/twit.md) and [Tech News Weekly](../shows/tnw.md) synthesize weekly industry announcements across competing ecosystems.[^archive-data]

# Landmark & Highest-Signal Episodes

The highest-signal episodes in the AI and Machine Learning cluster are split exclusively between [Security Now](../shows/sn.md) and [Intelligent Machines](../shows/im.md), illustrating how security threat analysis and dedicated AI news coverage jointly anchor the archive's deepest discussions.[^archive-data]

At the top of the list sits Security Now #1011 (191 keyword hits; 2025-02-04, *"Jailbreaking AI"*). Laporte opens by noting that *"It's almost all AI, all the time"* as Gibson examines AI jailbreaking and local inference.[^archive-data][^grc-sn] Highlighting the impact of open-weight models on self-hosting, Gibson observes:

> "And Leo, I will be talking about this later. But one of the things that DeepSeek has done has given people to run the models locally." — Steve Gibson [Security Now #1011, 2025-02-04, TS:N/A][^archive-data][^grc-sn]

Security Now #1093 (157 hits; 2026-08-25, *"Tokens in the Stream"*) extends that technical critique to a paper arguing that the underlying mechanism of an LLM is inherently insecure, while #1100 (135 hits; 2026-10-13, *"Booby Trapping LLMs"*) examines maliciously trained AI alongside a listener's ESP32-plus-LLM Halloween project. In #1100, Gibson underscores the unresolved safety challenge:

> "I don't think we have. I just think it's ultimately, we're going to— they're going to be turned— well, what we heard from OpenAI's chief scientist is that we really can't go much further until we get this under control." — Steve Gibson [Security Now #1100, 2026-10-13, TS:00:40:04][^archive-data][^grc-sn]

On the product and culture side, a four-week run of Intelligent Machines in February–March 2026 (#857 through #860) captures the rapid maturation of coding agents and vendor competition. In #858 (152 hits, Feb 18th 2026), Laporte, Jarvis, and PC Magazine's Emily Forlini cover OpenClaw creator Peter Steinberger joining OpenAI amid fierce Anthropic competition, with Forlini noting that OpenAI had narrowed from broad image and video spectacle because *"Now this week. They just want to compete with Anthropic."*[^archive-data] One week later, in #859 (174 hits, Feb 25th 2026, featuring Stack Exchange and Discourse creator Jeff Atwood), Laporte demonstrates Claude Code's new remote control feature while Martineau recounts an alarming agentic incident:

> "You know, she had to go run and unplug it. A similar thing happened with an OpenAI engineer this week where it, he had an OpenClaw instance running, I believe it was called, called, uh, some sort of pithy claw pun name. It accidentally ended up giving away $450,000 to just some dude on Twitter who asked. No, how? Real money? Real money? Well, it was Solana, but it was real money from his bank account." — Paris Martineau [Intelligent Machines #859, Feb 25th 2026, TS:02:17:23][^archive-data]

In #860 (150 hits, Mar 4th 2026), guest host Jason Hiner joins Jarvis, Martineau, and Dan Patterson to examine the Anthropic–Pentagon showdown, Claude becoming the most popular app in the world, and Perplexity competing with OpenClaw.[^archive-data]

| Show | Episode | Date | Title | Keyword Hits |
|---|---|---|---|---|
| [Security Now](../shows/sn.md) | #1011 | 2025-02-04 | Security Now 1011: Jailbreaking AI | 191 |
| [Intelligent Machines](../shows/im.md) | #859 | Feb 25th 2026 | Intelligent Machines 859 transcript | 174 |
| [Security Now](../shows/sn.md) | #1093 | 2026-08-25 | Security Now 1093: Tokens in the Stream | 157 |
| [Intelligent Machines](../shows/im.md) | #858 | Feb 18th 2026 | Intelligent Machines 858 transcript | 152 |
| [Intelligent Machines](../shows/im.md) | #860 | Mar 4th 2026 | Intelligent Machines 860 transcript | 150 |
| [Security Now](../shows/sn.md) | #1100 | 2026-10-13 | Security Now 1100: Booby Trapping LLMs | 135 |
| [Intelligent Machines](../shows/im.md) | #857 | Feb 11th 2026 | Intelligent Machines 857 transcript | 132 |

# Archive Methodology & Caveats

Counts in this article combine automated keyword matching across 3,350 official speaker-attributed transcripts (`data/*_Transcripts_*.md`) and 28 unattributed YouTube caption backfills (`data_youtube/*/*_yt.md`), as documented in the [TWiT Transcript Archive](../datasets/twit-transcript-archive.md) specification.[^archive-data][^yt-data][^dataset-doc] Several caveats apply when interpreting trends. First, while episode-level dates and titles for [Security Now](../shows/sn.md) (including #1011 on 2025-02-04 and #1093 on 2026-08-25) have been verified against GRC.com's annual archives, raw `data/SN_Transcripts_*.md` chunks lacking parsed date headers (`year == 0` on disk) are counted in all-time totals and episode rankings rather than in the annual trend table above.[^archive-data][^grc-sn][^dataset-doc] Second, official transcript coverage is thinner in 2020–2021 than in 2023–2026, amplifying the apparent steepness of post-2022 growth.[^dataset-doc] Third, later 2026 official transcripts carry an AI-generated transcription notice, and broad keyword patterns (such as `AI`) capture both dedicated technical segments and passing references.[^archive-data]

# See Also

- **Viewpoints:** [AI and LLMs](../viewpoints/ai-and-llms.md), [Windows and Microsoft Copilot](../viewpoints/windows-and-microsoft-copilot.md)
- **Entities:** [OpenAI](../entities/openai.md), [Anthropic](../entities/anthropic.md), [NVIDIA](../entities/nvidia.md), [Google](../entities/google.md), [Microsoft](../entities/microsoft.md)
- **Related Topics:** [Hardware and Chips](../topics/hardware-and-chips.md), [Windows and Microsoft](../topics/windows-and-microsoft.md), [Cybersecurity and Privacy](../topics/cybersecurity-and-privacy.md), [Tech Policy and Media](../topics/tech-policy-and-media.md)
- **Shows:** [Intelligent Machines](../shows/im.md), [Security Now](../shows/sn.md), [This Week in Tech](../shows/twit.md), [Windows Weekly](../shows/ww.md), [Tech News Weekly](../shows/tnw.md), [This Week in Google](../shows/twig.md)
- **People:** [Leo Laporte](../people/leo-laporte.md), [Jeff Jarvis](../people/jeff-jarvis.md), [Paris Martineau](../people/paris-martineau.md), [Paul Thurrott](../people/paul-thurrott.md), [Steve Gibson](../people/steve-gibson.md)
- **Dataset & References:** [TWiT Transcript Archive](../datasets/twit-transcript-archive.md), [Organizations and Tools](../references/organizations-and-tools.md), [Notable People](../references/notable-people.md)

[^archive-data]: Processed official TWiT transcript Markdown chunks (577 files, 3,350 episodes)
[^yt-data]: YouTube caption backfill transcripts (28 files, unattributed)
[^dataset-doc]: TWiT Transcript Archive dataset specification
[^grc-sn]: GRC.com Security Now transcript archive
