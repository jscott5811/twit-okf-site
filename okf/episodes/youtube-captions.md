---
type: episode-catalog
title: "YouTube Caption Backfill Episodes"
description: "Complete episode-level index of all 28 unattributed YouTube caption backfill transcripts (729,525 words, diarization: none) stored in data_youtube/."
tags: [twit, episodes, youtube-captions, unattributed]
generated:
  by: "antigravity/gemini-4-neon-medium"
  at: "2026-11-23T22:50:24Z"
sources:
  - id: "yt-captions"
    resource: "local archive data_youtube/*/*.md"
    title: "Extracted YouTube English caption transcripts (28 files, unattributed)"
---

This catalog indexes all **28** YouTube caption backfill transcripts (**729,525** total words, averaging **26,054 words** per episode) currently extracted into `data_youtube/` for the [TWiT Transcript Archive](../datasets/twit-transcript-archive.md), covering [This Week in Tech](../shows/twit.md).[^yt-captions]

## Era Overview & Highlights

Created to backfill episodes absent from `twit.tv`'s 241-page official transcript index, this catalog preserves **28** episodes extracted via `fetch_youtube_captions.py` before YouTube's `IpBlocked` rate limit halted further automated downloads. The extracted batch focuses on [This Week in Tech](../shows/twit.md), capturing classic early-era episodes alongside unarchived numbering gaps.[^yt-captions]

**Diarization caveat (`diarization: none`):** Unlike official `twit.tv` and GRC.com transcripts (which achieve ~99.1% named speaker attribution), YouTube auto-generated English captions provide a single undifferentiated text stream with **no speaker diarization**. Accordingly, these files contribute to topic and entity frequency tracking (where leading extracted terms include **Google** (26 eps), **Apple** (22 eps), **Facebook** (15 eps), **Microsoft** (12 eps), **iPhone** (11 eps), **Windows** (9 eps)) but are strictly excluded from per-person speaker rosters and attributed POV quotes.[^yt-captions]

The longest transcript in this YouTube caption batch is **TWIT Episode 10** (*The 10-Day Reply Guy - RAMageddon, HomeView, Ikigai, & the Flying Tesla Roadster*) at **34,657 words** (`data_youtube/TWIT/TWIT_10_yt.md`). Additional missing episodes discovered across 13 official TWiT YouTube channels are cataloged in `data_youtube/_catalog.json` for resumable future extraction.[^yt-captions]

## YouTube Caption Episode Index

| Show | Ep | Upload Date | Title | Words | Source File | Video URL | Top Keywords |
| :--- | ---: | :--- | :--- | ---: | :--- | :--- | :--- |
| `TWIT` | 3 | unknown | Princess Peach 3-Frame Vine Jump - Apple event preview, Apple vs. Epic, Proton gets Tim Berners-Lee | 28,461 | `data_youtube/TWIT/TWIT_3_yt.md` | [Watch](https://www.youtube.com/watch?v=D9dH2-CVrB0) | Apple, Google, iPhone, Amazon, Facebook |
| `TWIT` | 10 | unknown | The 10-Day Reply Guy - RAMageddon, HomeView, Ikigai, & the Flying Tesla Roadster | 34,657 | `data_youtube/TWIT/TWIT_10_yt.md` | [Watch](https://www.youtube.com/watch?v=winzpKpNhC0) | Apple, Starlink, NVIDIA, Amazon, Tesla |
| `TWIT` | 387 | unknown | This Week in Tech 387: A Year's Worth of Shrimp in Two Days | 26,177 | `data_youtube/TWIT/TWIT_387_yt.md` | [Watch](https://www.youtube.com/watch?v=aRPe1Sl9Ncw) | Google, Apple, Windows, iPad, iPhone |
| `TWIT` | 388 | unknown | This Week in Tech 388: Can't Stop The Balmer | 26,005 | `data_youtube/TWIT/TWIT_388_yt.md` | [Watch](https://www.youtube.com/watch?v=cFcNXc3_D54) | Facebook, iPad, Apple, iPhone, Google |
| `TWIT` | 389 | unknown | This Week in Tech 389: 73% Editorially Independent | 26,239 | `data_youtube/TWIT/TWIT_389_yt.md` | [Watch](https://www.youtube.com/watch?v=wlJqKtEEJ2w) | Facebook, iPhone, Apple, Android, Google |
| `TWIT` | 390 | unknown | This Week in Tech 390: Girly Pockets | 23,593 | `data_youtube/TWIT/TWIT_390_yt.md` | [Watch](https://www.youtube.com/watch?v=cUGaqUqjuRg) | Apple, iPhone, Microsoft, iPad, Google |
| `TWIT` | 391 | unknown | This Week in Tech 391: File:/// | 27,885 | `data_youtube/TWIT/TWIT_391_yt.md` | [Watch](https://www.youtube.com/watch?v=5r99PxUiXIQ) | Apple, Facebook, Microsoft, Amazon, Samsung |
| `TWIT` | 392 | unknown | This Week in Tech 392: I'm on the Board | 24,750 | `data_youtube/TWIT/TWIT_392_yt.md` | [Watch](https://www.youtube.com/watch?v=jIOmW8kclkM) | Apple, Microsoft, Windows, Google, Amazon |
| `TWIT` | 393 | unknown | This Week in Tech 393: Shrimp Fork to The Eye | 27,670 | `data_youtube/TWIT/TWIT_393_yt.md` | [Watch](https://www.youtube.com/watch?v=a_FdNwF2PUA) | Windows, Google, Apple, Microsoft, Tesla |
| `TWIT` | 394 | unknown | This Week in Tech 394: Math Has Sold Out | 26,206 | `data_youtube/TWIT/TWIT_394_yt.md` | [Watch](https://www.youtube.com/watch?v=Yi6ChNqADiE) | Google, Apple, Samsung, iPhone, Copyright |
| `TWIT` | 395 | unknown | This Week in Tech 395: It's Not Blue, It's Bluish | 24,052 | `data_youtube/TWIT/TWIT_395_yt.md` | [Watch](https://www.youtube.com/watch?v=dRjo0JcEU_A) | Apple, Google, Samsung, Android, Facebook |
| `TWIT` | 396 | unknown | This Week in Tech 396: A Segway for Your Face | 25,000 | `data_youtube/TWIT/TWIT_396_yt.md` | [Watch](https://www.youtube.com/watch?v=ympp9gnbC_Q) | Facebook, Google, Windows, Microsoft, iPad |
| `TWIT` | 397 | unknown | This Week in Tech 397: You+S=Us | 23,216 | `data_youtube/TWIT/TWIT_397_yt.md` | [Watch](https://www.youtube.com/watch?v=10HrOwoFtr8) | Google, Samsung, Android, Galaxy, iPhone |
| `TWIT` | 398 | unknown | This Week in Tech 398: Not My Toner! | 24,929 | `data_youtube/TWIT/TWIT_398_yt.md` | [Watch](https://www.youtube.com/watch?v=rLzl6pwupA8) | Google, Apple, iPad, YouTube, iPhone |
| `TWIT` | 399 | unknown | This Week in Tech 399: Look At That Codpiece | 23,342 | `data_youtube/TWIT/TWIT_399_yt.md` | [Watch](https://www.youtube.com/watch?v=fA9WG3kUkB0) | Google, Facebook, YouTube, Amazon, Android |
| `TWIT` | 400 | unknown | This Week in Tech 400: Live from Lake Tinky Winky | 29,264 | `data_youtube/TWIT/TWIT_400_yt.md` | [Watch](https://www.youtube.com/watch?v=5dfI-KEBeZA) | Apple, Facebook, Google, YouTube, Android |
| `TWIT` | 401 | unknown | This Week in Tech 401: Skip the Middle Man | 24,175 | `data_youtube/TWIT/TWIT_401_yt.md` | [Watch](https://www.youtube.com/watch?v=zSm6GhKCqZE) | Google, Facebook, Android, YouTube, Galaxy |
| `TWIT` | 402 | unknown | This Week in Tech 402: Wagner II: Electric Boogaloo | 28,447 | `data_youtube/TWIT/TWIT_402_yt.md` | [Watch](https://www.youtube.com/watch?v=_UTmqzCuEp8) | Apple, Google, Windows, Facebook, iPhone |
| `TWIT` | 403 | unknown | This Week in Tech 403: HP Smelt it | 25,662 | `data_youtube/TWIT/TWIT_403_yt.md` | [Watch](https://www.youtube.com/watch?v=pnCopTDnOqE) | Apple, Google, Windows, iPhone, iPad |
| `TWIT` | 404 | unknown | This Week in Tech 404: Episode Not Found | 25,514 | `data_youtube/TWIT/TWIT_404_yt.md` | [Watch](https://www.youtube.com/watch?v=mvlZeZbNths) | Google, Xbox, Apple, Facebook, Intel |
| `TWIT` | 405 | unknown | This Week in Tech 405: Only if You Follow Jerks | 23,570 | `data_youtube/TWIT/TWIT_405_yt.md` | [Watch](https://www.youtube.com/watch?v=2fr4xXGu2cU) | Windows, Google, Microsoft, YouTube, Apple |
| `TWIT` | 406 | unknown | This Week in Tech 406: Om in Yoga Pants | 26,009 | `data_youtube/TWIT/TWIT_406_yt.md` | [Watch](https://www.youtube.com/watch?v=7hMVuS6lqWk) | Google, Android, Facebook, Windows, YouTube |
| `TWIT` | 407 | unknown | This Week in Tech 407: Paleo Nostalgia | 27,236 | `data_youtube/TWIT/TWIT_407_yt.md` | [Watch](https://www.youtube.com/watch?v=lNPL11IoYm0) | Xbox, Google, Apple, Microsoft, iPhone |
| `TWIT` | 408 | unknown | This Week in Tech 408: NUC NUC NUC | 23,923 | `data_youtube/TWIT/TWIT_408_yt.md` | [Watch](https://www.youtube.com/watch?v=WAif8nQxfoE) | Google, Microsoft, Windows, Apple, Android |
| `TWIT` | 409 | unknown | This Week in Tech 409: Her Skin Bowls | 24,310 | `data_youtube/TWIT/TWIT_409_yt.md` | [Watch](https://www.youtube.com/watch?v=-twQA8F_tZ8) | Google, Apple, Facebook, Android, Microsoft |
| `TWIT` | 410 | unknown | This Week in Tech 410: Now With More Neck Stabbing | 26,600 | `data_youtube/TWIT/TWIT_410_yt.md` | [Watch](https://www.youtube.com/watch?v=RyZML_Jpin4) | Apple, Google, Xbox, iOS, Microsoft |
| `TWIT` | 411 | unknown | This Week in Tech 411: Inspired by Actual Events | 27,542 | `data_youtube/TWIT/TWIT_411_yt.md` | [Watch](https://www.youtube.com/watch?v=X3yzSe7XvTY) | Google, Facebook, Apple, Microsoft, Xbox |
| `TWIT` | 412 | unknown | This Week in Tech 412: Printed Pizza | 25,091 | `data_youtube/TWIT/TWIT_412_yt.md` | [Watch](https://www.youtube.com/watch?v=xUkIK_lURjs) | Facebook, Google, Microsoft, Galaxy, Encryption |

[^yt-captions]: Extracted directly from `data_youtube/*/*.md` frontmatter and caption text (28 files, 729,525 words, `diarization: none`).
