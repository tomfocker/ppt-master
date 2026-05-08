# Style Sample Library

This directory stores reusable raster reference samples for PPT Master template design.

These images are not layout templates themselves. They are visual direction boards for:

- creating new `layouts/` templates
- choosing a presentation style during the Strategist phase
- giving the Executor a concrete visual reference when a user asks for a style such as "consulting", "medical", "dark AI engineering", or "Zen"

All samples are 16:9 PNG images generated with Codex native image generation and copied into this repository for reuse.

## Usage

When a user asks for a style that matches one of these samples:

1. Use the image only as a visual reference.
2. Do not copy raster text or screenshot-like elements directly into final PPT pages.
3. Rebuild the actual slides as editable SVG / DrawingML-compatible shapes.
4. Keep the final SVG compliant with `references/shared-standards.md` and `SKILL.md`.
5. Avoid real logos, real seals, readable fake text, and copyrighted brand marks unless the user provides explicit source material and rights.

## Sample Index

| Sample | Preview | Best For | Visual Direction |
|--------|---------|----------|------------------|
| `风格_高端咨询` | ![](./images/consulting_executive_sample.png) | Strategy consulting, board reports, investment analysis | Deep navy, white canvas, precise grids, executive hierarchy, restrained gold/cyan accents |
| `government_red` | ![](./images/government_red_sample.png) | Government reports, SOE briefings, party/governance-adjacent formal reports | Deep red, ivory, muted gold, symmetrical structure, official document rhythm |
| `风格_暗色AI工程` | ![](./images/dark_ai_engineering_sample.png) | AI safety, engineering architecture, system reviews, developer talks | Near-black, slate panels, blue/cyan diagrams, risk and architecture modules |
| `academic_research` | ![](./images/academic_research_sample.png) | Thesis defense, academic reports, research proposals | University blue, scholarly grid, methodology and finding blocks, citation-like footers |
| `medical_university` | ![](./images/medical_university_sample.png) | Hospital reports, case discussions, clinical research | Medical blue, white clinical canvas, protocol flows, case and metrics panels |
| `风格_高端金融` | ![](./images/premium_finance_sample.png) | Banking, wealth management, transaction finance, executive finance reports | Bank red, pearl white, graphite, gold accents, borderless premium modules |
| `tech_annual_report` | ![](./images/tech_annual_report_sample.png) | Tech annual reports, team reviews, product analytics, OKR summaries | Bright white, four-color accents, modular dashboard cards, friendly data storytelling |
| `psychology_counseling` | ![](./images/psychology_counseling_sample.png) | Psychology courses, counseling training, attachment theory | Teal/blue-green warmth, soft panels, relationship maps, reflective learning cards |
| `pixel_retro_training` | ![](./images/pixel_retro_training_sample.png) | Developer onboarding, Git training, gamified tech education | Pixel borders, dark grid, neon green/magenta/cyan, level-map learning rhythm |
| `风格_禅意经典` | ![](./images/zen_classics_sample.png) | Classical text study, philosophy, traditional culture lectures | Ink-wash restraint, warm paper, moss green, cinnabar accent, large negative space |
| `风格_能源基建` | ![](./images/energy_infrastructure_sample.png) | Infrastructure strategy, energy projects, international engineering | Deep sea blue, consulting modules, risk matrix, project map and financial sensitivity rhythm |
| `automotive_certification` | ![](./images/automotive_certification_sample.png) | Automotive testing, certification institutes, green mobility strategy | Deep blue, cyan and green accents, testing pipeline, certification matrix, roadmap modules |

## Prompt Pattern

Use this pattern when extending the library:

```text
Use case: productivity-visual
Asset type: reusable PPT template reference sample, 16:9 widescreen theme board
Primary request: Create a polished reference sample image for a <domain/style> presentation theme. It should be a reusable visual direction for PPT Master templates, not a finished slide with readable copy.
Scene/backdrop: <domain atmosphere>
Subject: abstract PowerPoint-style layout preview with <relevant page modules>
Composition: 16:9, <layout rhythm>
Style: <style language>
Color palette: <core colors>
Text: no readable text, only abstract placeholder lines and blocks.
Avoid: logos, brand names, readable text, watermarks, people unless explicitly required.
```

## File Naming

Use lowercase snake_case:

```text
<style_slug>_sample.png
```

Keep generated source files in the Codex default directory and copy selected final assets here. Do not delete the original generated files unless explicitly requested.
