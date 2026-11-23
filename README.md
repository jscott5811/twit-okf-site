# TWiT Knowledge Base (Open Knowledge Format v0.3)

An independent, non-commercial **Open Knowledge Format (OKF v0.3)** encyclopedia, metadata index, and topical reference guide covering 18 shows and 3,378 archived episodes across the [TWiT.tv](https://twit.tv/) podcast network.

> **Important Notice — No Raw Transcripts Published:**
> **No raw transcripts are published or redistributed** in this repository or on the GitHub Pages site. This repository contains only structured OKF v0.3 metadata, aggregated topic/entity/domain analytics, episode catalog indices, and brief attributed quotations for commentary and reference.

## What's Inside (`okf/`)

- **96 OKF v0.3 Concepts (107 Markdown files, ~224,000 words):**
  - `okf/shows/` — 18 Wikipedia-style show profiles covering every `SHOW_MAP` prefix (`AAA` through `WW`), with official `twit.tv` URLs, launch dates, and publication status.
  - `okf/episodes/` — 24 episode catalogs indexing 3,350 official episodes (100% dated; 0 undated) + 28 unattributed YouTube caption backfills.
  - `okf/people/` — 20 biographies of recurring TWiT hosts, panelists, journalists, and security researchers with verbatim attributed stances.
  - `okf/viewpoints/` — 7 cross-host topical debate articles contrasting host perspectives side-by-side.
  - `okf/entities/` — 12 organization and ecosystem profiles with 2020–2026 mention trends.
  - `okf/topics/` — 9 technology, science, security, and policy topic clusters.
  - `okf/references/` — 4 catalogs of recurring non-sponsor domains, publications, organizations, and notable people.
  - `okf/datasets/` & `okf/playbooks/` — Archive schema specification and operational sync documentation.

## Attribution & License

Underlying TWiT public streams and on-demand shows are produced by **TWiT LLC** ([https://twit.tv/](https://twit.tv/)) and released under the **Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International (CC BY-NC-ND 4.0)** license ([https://creativecommons.org/licenses/by-nc-nd/4.0/](https://creativecommons.org/licenses/by-nc-nd/4.0/)). Legacy *Security Now* transcripts are credited to **Steve Gibson / Gibson Research Corporation** ([https://www.grc.com/](https://www.grc.com/)).

See [ATTRIBUTION.md](ATTRIBUTION.md) for full licensing, attribution, and non-redistribution details.

## Publishing & Local Preview

This repository deploys automatically to **GitHub Pages** via `.github/workflows/pages.yml` using **MkDocs Material** (`mkdocs.yml`, `docs_dir: okf`).

To preview locally:

```bash
pip install mkdocs-material
mkdocs serve
```

To validate OKF v0.3 conformance:

```bash
python /path/to/open-knowledge-format/skills/okf-generate/scripts/validate.py okf --strict
```
