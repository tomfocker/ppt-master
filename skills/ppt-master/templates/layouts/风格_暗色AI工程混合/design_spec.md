# Dark AI Engineering Hybrid - Design Specification

> Hybrid visual template for AI safety, architecture reviews, and engineering deep dives. Raster backgrounds provide native-image atmosphere; all titles, labels, content cards, diagrams, and metrics are editable SVG / DrawingML overlay elements.

## I. Template Overview

| Property | Description |
| --- | --- |
| Template ID | `风格_暗色AI工程混合` |
| Template Name | Dark AI Engineering Hybrid |
| Category | Special / Hybrid Visual |
| Use Cases | AI safety review, system architecture, developer conference, technical postmortem |
| Design Tone | Premium, cinematic, technical, dark, precise |
| Theme Mode | Hybrid: raster atmosphere background + editable SVG information layer |

## II. Canvas Specification

| Property | Value |
| --- | --- |
| Format | PPT 16:9 |
| Dimensions | 1280 x 720 px |
| viewBox | `0 0 1280 720` |

## III. Assets

| Asset | Purpose |
| --- | --- |
| `assets/cover_bg.png` | Cover / chapter / ending atmosphere background |
| `assets/content_bg.png` | Content page low-contrast technical background |

## IV. Color Scheme

| Role | Value |
| --- | --- |
| Background | `#0B1020` |
| Panel | `#0F172A` |
| Panel Strong | `#111827` |
| Primary | `#58A6FF` |
| Accent | `#22D3EE` |
| Warning | `#F59E0B` |
| Success | `#34D399` |
| Danger | `#F97373` |
| Text | `#FFFFFF` |
| Muted | `#8B9BB4` |
| Line | `#243044` |

## V. Typography System

Font stack: `PingFang SC, Microsoft YaHei, Arial, sans-serif`.

| Level | Size | Usage |
| --- | ---: | --- |
| Cover title | 50-56px | Main title |
| Page title | 26px | Content title |
| Key message | 18px | Takeaway bar |
| Body | 14-16px | Cards and annotations |
| Footer | 10-12px | Source and page number |

## VI. Page Types

| File | Purpose |
| --- | --- |
| `01_cover.svg` | Cover using `cover_bg.png` plus editable text |
| `02_toc.svg` | TOC using `content_bg.png` plus editable TOC cards |
| `02_chapter.svg` | Chapter page using `cover_bg.png` plus editable chapter text |
| `03_content.svg` | Content page using `content_bg.png` plus editable key message and flexible content area |
| `04_ending.svg` | Ending page using `cover_bg.png` plus editable closing text |

## VII. Hybrid Rules

- The background image is intentionally not editable; it carries atmosphere only.
- All information-bearing content must be editable SVG text, shapes, lines, charts, and cards.
- Do not place important text directly inside the background image.
- Keep central content overlays on semi-transparent dark panels to maintain readability.

## VIII. SVG Technical Constraints

- Use direct SVG attributes only.
- Do not use `<style>`, `class`, `<foreignObject>`, masks, scripts, animations, or `<g opacity>`.
- Use `<image>` only for the two local background assets.

## IX. Placeholder Specification

`{{TITLE}}`, `{{SUBTITLE}}`, `{{DATE}}`, `{{AUTHOR}}`, `{{CHAPTER_NUM}}`, `{{CHAPTER_TITLE}}`, `{{CHAPTER_DESC}}`, `{{PAGE_TITLE}}`, `{{KEY_MESSAGE}}`, `{{CONTENT_AREA}}`, `{{SOURCE}}`, `{{PAGE_NUM}}`, `{{THANK_YOU}}`, `{{CONTACT_INFO}}`, `{{TOC_ITEM_N_TITLE}}`, `{{TOC_ITEM_N_DESC}}`.
