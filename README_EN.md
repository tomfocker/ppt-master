# PPT Master Fork

This repository is a fork of [hugohe3/ppt-master](https://github.com/hugohe3/ppt-master). It keeps the original workflow for generating natively editable PPTX files from PDF, DOCX, URL, and Markdown sources, and adds reusable template assets on top.

> The original project is created and maintained by Hugo He under the MIT License. This fork focuses on reusable template expansion.

English | [中文](./README.md)

---

## What This Fork Adds

### 1. Example-Derived Templates

This fork turns selected high-quality `examples/` projects into reusable layout templates under:

```text
skills/ppt-master/templates/layouts/
```

These templates preserve the original visual language, page structure, and pacing, while replacing project-specific content with reusable placeholders.

New example-derived templates include:

| Template | Use cases |
|----------|-----------|
| `示例_项目介绍` | Product intros, project pitches, internal briefings |
| `示例_暗色科技自动模式` | AI safety, engineering architecture, R&D sharing |
| `示例_像素风Git入门` | Technical training, developer onboarding |
| `示例_易理风谦卦` | Traditional culture, philosophy, humanities lectures |
| `示例_禅意风金刚经` | Buddhist studies, classic text reading, cultural courses |
| `示例_谷歌风年度报告` | Annual reports, team reviews, project summaries |
| `示例_暗色代码调试` | Developer training, debugging methodology |
| `示例_技术对比AI编程工具` | Tool reviews, competitive analysis, technical selection |
| `示例_咨询风依恋心理` | Psychology courses, counseling training |
| `示例_咨询风AI代理` | AI agents, architecture, technical strategy |
| `示例_咨询风甘孜财政` | Fiscal analysis, regional economy, government reports |
| `示例_咨询风重庆区域` | Regional research, finance, risk analysis |
| `示例_高端咨询南欧江` | Infrastructure, energy projects, international engineering |
| `示例_高端咨询汽车认证` | Five-year plans, automotive certification, strategy |
| `示例_麦肯锡客户忠诚` | Customer research, loyalty analysis, business strategy |

### 2. Expanded Layout Library

The layout library now contains 43 templates across brand, government, business, academic, medical, psychology, example-derived, and style-library templates.

See:

- [Template README](./skills/ppt-master/templates/layouts/README.md)
- [Machine-readable index](./skills/ppt-master/templates/layouts/layouts_index.json)

### 3. Style Sample Library

This fork adds a set of 16:9 raster style reference boards for new template design, style selection, and visual alignment. These samples are not final PPT pages; rebuild them as editable SVG / DrawingML elements when creating slides.

- [Style Sample README](./skills/ppt-master/templates/style_samples/README.md)
- [Style sample index](./skills/ppt-master/templates/style_samples/style_samples_index.json)

Seven high-frequency directions have also been converted into directly usable `layouts/` templates: `premium_finance`, `dark_ai_engineering`, `dark_ai_engineering_hybrid`, `consulting_executive`, `government_red_modern`, `zen_classics`, and `energy_infrastructure`.

`dark_ai_engineering_hybrid` is a hybrid template: raster-generated backgrounds provide stronger native image quality, while titles, cards, metrics, and charts remain editable SVG / DrawingML information layers.

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

### 3. Ask an AI Agent

The upstream project already provides [AGENTS.md](./AGENTS.md) as the entry point for general AI agents. When using this fork, still ask the agent to read `AGENTS.md` and `skills/ppt-master/SKILL.md` before generation.

Free design:

```text
Please read AGENTS.md and skills/ppt-master/SKILL.md,
then create a 16:9 PPT from projects/my-report/sources/report.pdf.
```

Use one of this fork's new templates:

```text
Please read AGENTS.md and skills/ppt-master/SKILL.md,
use the 「示例_麦肯锡客户忠诚」 template,
and create a 16:9 PPT from projects/customer-research/sources/report.pdf.
```

Use an existing upstream template:

```text
Please use the mckinsey template for a consulting-style deck.
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

## Common Commands

Initialize a project:

```bash
python3 skills/ppt-master/scripts/project_manager.py init my_deck --format ppt169
```

Import sources:

```bash
python3 skills/ppt-master/scripts/project_manager.py import-sources projects/my_deck path/to/source.pdf --move
```

Validate:

```bash
python3 skills/ppt-master/scripts/project_manager.py validate projects/my_deck
```

Export, one command at a time:

```bash
python3 skills/ppt-master/scripts/total_md_split.py projects/my_deck
```

```bash
python3 skills/ppt-master/scripts/finalize_svg.py projects/my_deck
```

```bash
python3 skills/ppt-master/scripts/svg_to_pptx.py projects/my_deck -s final
```

---

## Upstream Sync

This fork tracks the original project as upstream:

```text
upstream: https://github.com/hugohe3/ppt-master
origin:   https://github.com/tomfocker/ppt-master
```

To sync upstream changes:

```bash
git fetch upstream
git merge upstream/main
```

---

## Key Docs

| Document | Description |
|----------|-------------|
| [AGENTS.md](./AGENTS.md) | Entry point for general AI coding agents |
| [SKILL.md](./skills/ppt-master/SKILL.md) | Full PPT Master workflow |
| [Template README](./skills/ppt-master/templates/layouts/README.md) | Template list and structure |
| [Scripts README](./skills/ppt-master/scripts/README.md) | Conversion, project, and export tools |
| [FAQ](./docs/faq.md) | Troubleshooting |

---

## License

This fork inherits the original MIT License. Copyright and attribution for the original project belong to Hugo He and contributors.
