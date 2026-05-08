# 高端金融混合 - Design Specification

> Hybrid visual template for private banking, wealth management, transaction finance, and executive finance reports. Raster backgrounds provide premium atmosphere; all titles, labels, content cards, diagrams, and metrics are editable SVG / DrawingML overlay elements.

## I. Template Overview

| Property | Description |
| --- | --- |
| Template ID | `风格_高端金融混合` |
| Template Name | 高端金融混合 |
| Category | Special / Hybrid Visual |
| Use Cases | 银行方案、财富管理、交易银行、金融高管汇报 |
| Design Tone | Premium, financial, restrained, elegant, authoritative |
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
| Background | `#101114` |
| Panel | `#181A20` |
| Panel Strong | `#222025` |
| Primary | `#B9975B` |
| Accent | `#C8A35D` |
| Warning | `#D6A84F` |
| Success | `#3FBF8F` |
| Danger | `#B91C1C` |
| Text | `#FFFFFF` |
| Muted | `#C8CED8` |
| Line | `#3A312A` |

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
