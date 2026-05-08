# PPT Master Fork

This repository is a fork of [hugohe3/ppt-master](https://github.com/hugohe3/ppt-master). It keeps the upstream workflow for generating natively editable PPTX files from PDF, DOCX, URL, and Markdown sources, and adds a Chinese-first reusable template library on top.

> The original project is created and maintained by Hugo He under the MIT License. This fork focuses on reusable template expansion, Chinese-readable template IDs, and hybrid visual templates.

English | [中文](./README.md)

---

## Sync Status

This fork has been synced with the upstream v2.6.0-era capabilities while preserving this fork's template-library additions.

Upstream capabilities now included here include:

- PPTX template import and replication: extract masters, layouts, assets, and reusable template structure from existing `.pptx` files.
- Better PPTX / SVG round-trip fidelity for image crops, theme backgrounds, tables, placeholders, nested SVG, and picture transforms.
- New workflows: `topic-research`, `resume-execute`, `verify-charts`, `visual-edit`, and `generate-audio`.
- Documentation and tooling for animations, transitions, narration, audio, and video export.
- Expanded examples, online preview indexing, and icon library updates.

---

## What This Fork Adds

### 1. Chinese-First Reusable Templates

This fork turns selected high-quality `examples/` projects into reusable layout templates under:

```text
skills/ppt-master/templates/layouts/
```

These templates preserve the original visual language, page structure, and pacing, while replacing project-specific content with reusable placeholders.

### 2. Expanded Layout Library

The layout library now contains 46 templates across upstream brand, government, business, academic, medical, psychology, example-derived, and style-library templates.

See:

- [Template README](./skills/ppt-master/templates/layouts/README.md)
- [Machine-readable index](./skills/ppt-master/templates/layouts/layouts_index.json)

### 3. Style Samples And Hybrid Templates

This fork adds a set of 16:9 raster style reference boards for new template design, style selection, and visual alignment.

- [Style Sample README](./skills/ppt-master/templates/style_samples/README.md)
- [Style sample index](./skills/ppt-master/templates/style_samples/style_samples_index.json)

Hybrid templates use raster-generated backgrounds for stronger visual quality while keeping titles, cards, metrics, and charts as editable SVG / DrawingML information layers.

---

## Usage

### 1. Install

Requires Python 3.10+.

```bash
pip install -r requirements.txt
```

Windows users can follow:

- [Windows Installation Guide](./docs/windows-installation.md)

### 2. Add Source Materials

Put PDF, DOCX, Markdown, images, or other source files under `projects/`, for example:

```text
projects/my-report/sources/report.pdf
```

### 3. Ask An AI Agent

When using this fork, ask the agent to read `AGENTS.md` and `skills/ppt-master/SKILL.md` before generation.

Free design:

```text
Please read AGENTS.md and skills/ppt-master/SKILL.md,
then create a 16:9 PPT from projects/my-report/sources/report.pdf.
```

Use one of this fork's templates:

```text
Please read AGENTS.md and skills/ppt-master/SKILL.md,
use the 「风格_暗色AI工程混合」 template,
and create a 16:9 PPT from projects/ai-review/sources/report.pdf.
```

> Template usage is opt-in. If you do not name a template, the workflow defaults to free design.

### 4. Output

Generated files are saved under the project's `exports/` directory:

```text
*.pptx
*_svg.pptx
```

- `.pptx`: natively editable PowerPoint shapes
- `_svg.pptx`: visual reference version

---

## Keeping Upstream Sync

```text
upstream: https://github.com/hugohe3/ppt-master
origin:   https://github.com/tomfocker/ppt-master
```

```bash
git fetch upstream
git merge upstream/main
```

---

## License

This fork inherits the original MIT License. Original copyright and attribution belong to Hugo He and contributors.
