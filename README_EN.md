# PPT Master Fork

[![Version](https://img.shields.io/badge/version-v2.9.0-blue.svg)](https://github.com/hugohe3/ppt-master/releases)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

[中文](./README.md) | English

This repository is a fork of [hugohe3/ppt-master](https://github.com/hugohe3/ppt-master). It keeps the upstream workflow for generating natively editable PowerPoint files from PDFs, DOCX files, URLs, Markdown, and PPTX templates, while adding a Chinese-first reusable template and style library.

The fork is currently synced with upstream v2.9.0-era capabilities, including direct PPTX template fill, the brand/layout/deck template split, live preview editing, visual review, LaTeX rendering, animation/narration improvements, 71 visualization templates, and the expanded example catalog.

## What This Fork Adds

- Chinese-first README and template usage notes.
- Reusable template assets organized as `templates/brands/`, `templates/layouts/`, and `templates/decks/`.
- Chinese-readable example-derived layouts such as `示例_麦肯锡客户忠诚` and style layouts such as `风格_暗色AI工程混合`.
- A raster style-sample library under `templates/style_samples/` for reusable visual direction.
- Hybrid templates that use generated bitmap backgrounds for atmosphere while keeping text, cards, metrics, charts, and diagrams editable as SVG / DrawingML layers.

## Usage

Install dependencies:

```bash
pip install -r requirements.txt
```

Ask the agent to read `AGENTS.md` and `skills/ppt-master/SKILL.md` before generation:

```text
Read AGENTS.md and skills/ppt-master/SKILL.md, then generate a 16:9 deck from projects/my-report/sources/report.pdf.
```

Use a fork template by explicit path:

```text
Use template path skills/ppt-master/templates/layouts/风格_暗色AI工程混合/ and generate a deck from projects/ai-review/sources/report.pdf.
```

Template selection is opt-in by full directory path. Bare names are useful for discussion and discovery, but they do not trigger the template workflow.

## Key Paths

| Path | Purpose |
|------|---------|
| `AGENTS.md` | Agent entry rules |
| `skills/ppt-master/SKILL.md` | Main PPT generation workflow |
| `skills/ppt-master/workflows/` | Standalone workflows |
| `skills/ppt-master/templates/` | Brands, layouts, decks, style samples, charts, and icons |
| `examples/` | Example projects and fork template previews |
| `projects/` | Local project workspace |

## License

This fork inherits the upstream MIT License. Original project copyright and attribution belong to Hugo He and contributors.
