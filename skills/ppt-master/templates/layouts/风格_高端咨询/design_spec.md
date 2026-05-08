# Consulting Executive - Design Specification

> High-end executive consulting template for board reports, strategy decks, and investment analysis.

## I. Template Overview

| Property | Description |
| --- | --- |
| Template ID | `风格_高端咨询` |
| Template Name | Consulting Executive |
| Category | General |
| Use Cases | Board report, strategy consulting, investment analysis, executive presentation, market study |
| Design Tone | Structured, precise, premium, data-driven, conclusion-first |
| Theme Mode | Light executive theme with deep navy system and restrained accents |
| Reference Sample | `../style_samples/images/consulting_executive_sample.png` |

## II. Canvas Specification

| Property | Value |
| --- | --- |
| Format | PPT 16:9 |
| Dimensions | 1280 x 720 px |
| viewBox | `0 0 1280 720` |
| Safe Area | x: 56-1224, y: 48-672 |

## III. Color Scheme

| Role | Value | Usage |
| --- | --- | --- |
| Background | `#FFFFFF` | Main light canvas or page base |
| Dark | `#061A33` | Dark page backgrounds and primary text |
| Primary | `#005587` | Structural bars, title accents |
| Secondary | `#EEF3F8` | Cards and soft panels |
| Accent | `#D9A441` | Dividers, highlights, key markers |
| Muted Text | `#6B7280` | Subtitles, metadata, footer text |
| Panel | `#F8FAFC` | Content containers |
| Line | `#DDE5EE` | Rules, borders, dividers |

## IV. Typography System

| Level | Size | Weight | Usage |
| --- | ---: | --- | --- |
| Cover title | 56px | Bold | `{{TITLE}}` |
| Chapter title | 48px | Bold | `{{CHAPTER_TITLE}}` |
| Page title | 26px | Bold | `{{PAGE_TITLE}}` |
| Key message | 18px | Bold | `{{KEY_MESSAGE}}` |
| Body | 16-18px | Regular | Generated content |
| Footer | 10-12px | Regular | Source, section, page number |

Font stack: `Arial, "Helvetica Neue", sans-serif`.

## V. Page Structure

- Top structural bar defines template identity.
- Cover, chapter, and ending pages establish the emotional tone.
- Content page keeps a flexible editable content area and only fixes header, key message, footer, and light scaffolding.
- Use the reference sample as a style guide only; final pages must be rebuilt as editable SVG elements.

## VI. Page Types

| File | Purpose |
| --- | --- |
| `01_cover.svg` | Cover page with title, subtitle, author, date |
| `02_toc.svg` | Table of contents with six indexed items |
| `02_chapter.svg` | Chapter divider with number and title |
| `03_content.svg` | Flexible content page with key message bar |
| `04_ending.svg` | Ending page with thank-you and contact info |

## VII. Layout Modes (Recommended)

| Mode | Use Case |
| --- | --- |
| `anchor` | One key visual, hero message, cover-like content pages |
| `dense` | Tables, KPIs, matrices, multi-module analysis |
| `breathing` | Quotes, conclusions, cultural or reflective pages |

## VIII. Spacing Specification

- Outer margin: 56px.
- Header height: 64-84px.
- Main content zone: y=168-598.
- Footer baseline: y=678.
- Card radius: 6-16px depending on page tone.

## IX. SVG Technical Constraints

- viewBox must be `0 0 1280 720`.
- Do not use `<style>`, `class`, external CSS, `<foreignObject>`, scripts, animation, masks, or embedded iframes.
- Use direct SVG attributes for fill, stroke, font, opacity, and geometry.
- Do not paste the raster style sample into final generated slides unless the user explicitly asks for image-based reference pages.

## X. Placeholder Specification

| Placeholder | Purpose |
| --- | --- |
| `{{TITLE}}` | Cover title |
| `{{SUBTITLE}}` | Cover subtitle |
| `{{DATE}}` | Date |
| `{{AUTHOR}}` | Author or organization |
| `{{CHAPTER_NUM}}` | Chapter number |
| `{{CHAPTER_TITLE}}` | Chapter title |
| `{{CHAPTER_DESC}}` | Chapter description |
| `{{PAGE_TITLE}}` | Content page title |
| `{{KEY_MESSAGE}}` | Key takeaway |
| `{{CONTENT_AREA}}` | Flexible AI-generated content area |
| `{{SECTION_NAME}}` | Footer section label |
| `{{SOURCE}}` | Footer source |
| `{{PAGE_NUM}}` | Page number |
| `{{THANK_YOU}}` | Ending message |
| `{{CONTACT_INFO}}` | Contact details |
| `{{TOC_ITEM_N_TITLE}}` | TOC item title, indexed 1-6 |
| `{{TOC_ITEM_N_DESC}}` | TOC item description, indexed 1-6 |
