# 现代政企红混合 - Design Specification

> Hybrid visual template for government reports, SOE briefings, policy communication, and formal annual summaries. Raster backgrounds provide dignified official atmosphere; all titles, labels, content cards, diagrams, and metrics are editable SVG / DrawingML overlay elements.

## I. Template Overview

| Property | Description |
| --- | --- |
| Template ID | `风格_现代政企红混合` |
| Template Name | 现代政企红混合 |
| Category | Special / Hybrid Visual |
| Use Cases | 政府报告、国企汇报、政策沟通、年度总结 |
| Design Tone | Formal, dignified, modern, warm, authoritative |
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
| Background | `#FFF8EC` |
| Panel | `#FFFFFF` |
| Panel Strong | `#FFF3E0` |
| Primary | `#9B111E` |
| Accent | `#C8A35D` |
| Warning | `#C8A35D` |
| Success | `#2E7D57` |
| Danger | `#B42318` |
| Text | `#5B0B10` |
| Muted | `#7B6B5D` |
| Line | `#E8DCC8` |

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
