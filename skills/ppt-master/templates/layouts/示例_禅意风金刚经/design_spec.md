# 禅意风金刚经示例模板 - Design Specification

> 从金刚经研究案例抽象出的禅意留白与经典研读模板。

## I. Template Overview

- Template ID: `示例_禅意风金刚经`
- Source example: `ppt169_禅意风_金刚经第一品研究`
- Category: Special
- Applicable scenarios: 佛学讲座、经典研读、文化课程、哲学分享
- Design tone: 留白、宁静、东方美学，适合慢节奏的文本阐释
- Theme mode: Light theme

## II. Canvas Specification

- Format: PPT 16:9
- ViewBox: `0 0 1280 720`
- Width: 1280
- Height: 720

## III. Color Scheme

- Primary: `#6B7A5A`
- Secondary: `#2E3A32`
- Accent: `#B08D57`
- Background: `#F7F4EA`
- Surface: `#FFFDF6`
- Text: `#27332B`

## IV. Typography System

- Primary font stack: `Microsoft YaHei`, `PingFang SC`, `Noto Sans CJK SC`, `Arial`, sans-serif
- Cover title: 54-68px, bold
- Section title: 44-56px, bold
- Page title: 28-36px, bold
- Body text: 18-24px
- Caption/footer text: 12-14px

## V. Page Structure

This template keeps the visual language of the source example but removes project-specific copy and data. It uses a consistent header/footer system, strong content margins, and reusable decorative motifs.

## VI. Page Types

- `01_cover.svg`: cover page with title, subtitle, date, and author placeholders
- `02_toc.svg`: table of contents page using indexed TOC placeholders
- `02_chapter.svg`: chapter divider page
- `03_content.svg`: content scaffold with page title and content area placeholder
- `04_ending.svg`: closing page with thank-you and contact placeholders

## VII. Layout Modes (Recommended)

- Anchor: one dominant insight with a supporting chart or visual
- Dense: structured tables, KPI blocks, or comparison matrices
- Breathing: transition, reflection, chapter, and summary pages

## VIII. Spacing Specification

- Outer margin: 64px
- Header area: 72px
- Footer area: 42px
- Content area: x=80, y=150, width=1120, height=470
- Card gap: 20-28px

## IX. SVG Technical Constraints

- Canvas must use `viewBox="0 0 1280 720"`
- Do not use `<style>`, `class`, `<foreignObject>`, scripts, animations, or external CSS
- Use direct SVG attributes for fill, stroke, opacity, and typography
- Keep images optional and local to the template package if introduced later

## X. Placeholder Specification

- Cover: `{{TITLE}}`, `{{SUBTITLE}}`, `{{DATE}}`, `{{AUTHOR}}`
- TOC: `{{TOC_ITEM_1_TITLE}}` through `{{TOC_ITEM_5_TITLE}}`, with matching `{{TOC_ITEM_N_DESC}}`
- Chapter: `{{CHAPTER_NUM}}`, `{{CHAPTER_TITLE}}`
- Content: `{{PAGE_TITLE}}`, `{{CONTENT_AREA}}`, `{{PAGE_NUM}}`, optional `{{SOURCE}}`
- Ending: `{{THANK_YOU}}`, `{{CONTACT_INFO}}`

## XI. Usage Guide

Use this template when a future project should borrow the source example's overall style without inheriting its original topic, data, or slide-specific content. Replace placeholders during the Strategist/Executor flow and keep the same color/spacing rhythm for consistency.
