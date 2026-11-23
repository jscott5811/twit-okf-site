# Bundle history

## 2026-11-23

* **Wikipedia-Style Encyclopedic Expansion**: Rewrote all concept articles across the entire 108-file OKF v0.3 bundle into detailed, source-backed Wikipedia-style articles featuring multi-paragraph leads, Quick Facts infoboxes, historical era narratives, cross-show editorial analysis, contextualized verbatim transcript excerpts, methodology caveats, and `See Also` cross-links:
  - Expanded all 12 [Entities](entities/index.md), all 9 [Topics](topics/index.md), all 4 [References](references/index.md), [TWiT Transcript Archive](datasets/twit-transcript-archive.md), and [Sync and Process Archive](playbooks/sync-and-process-archive.md) (27 files: 15,062 → 52,060 words, 3.46× growth).
  - Expanded all 18 [Shows](shows/index.md) and added era overview narratives across all 25 [Episodes](episodes/index.md) catalogs (preserving all 3,350 official + 28 YouTube = 3,378 episode rows).
  - Expanded all 20 [People](people/index.md) biographies and all 7 [Viewpoints](viewpoints/index.md) debate articles with contextualized verbatim attributed quotes from the 3,350 official transcripts.
* **Full-Archive + YouTube Caption Refresh**: Re-mined all 577 official Markdown chunks (3,350 episodes, 64,082,577 words after exhausting `twit.tv` pages 201–241) plus 28 YouTube caption backfills (`data_youtube/TWIT/`, 729,525 words) across all OKF concepts:
  - Updated [TWiT Transcript Archive](datasets/twit-transcript-archive.md), all 12 [Entities](entities/index.md), all 9 [Topics](topics/index.md), and all 4 [References](references/index.md) with combined official + YouTube caption counts and full 2014–2026 volume.
  - Re-mined all 20 [People](people/index.md) profiles and 7 [Viewpoints](viewpoints/index.md) strictly from the 3,350 speaker-attributed official episodes (excluding unattributed YouTube captions).
  - Updated [Sync and Process Archive](playbooks/sync-and-process-archive.md) with `fetch_youtube_captions.py` discovery and resumable batch extraction instructions.
* **Viewpoints & Verbatim Quotes**: Enriched all 20 [People](people/index.md) profiles with verbatim attributed points of view and added [Viewpoints](viewpoints/index.md) with 7 cross-host comparison concepts.
* **Deep Enrichment**: Added [People](people/index.md), [Entities](entities/index.md), [Episodes](episodes/index.md), and recorded user editorial note (2026-11-23) that [iOS Today](shows/ios.md), [Hands-On Tech](shows/hot.md), and out-of-scope show Home Theater Geeks have completed their runs.
* **Creation**: Generated initial OKF v0.3 knowledge base for the TWiT transcript archive.
