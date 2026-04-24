# 高端咨询汽车认证示例模板 - Design Specification

> 从汽车认证五年战略规划案例抽象出的认证机构战略规划模板。

## I. Template Overview

- Template ID: `示例_高端咨询汽车认证`
- Source example: `ppt169_高端咨询风_汽车认证五年战略规划`
- Category: Scenario
- Applicable scenarios: 五年规划、认证检测、汽车产业、绿色低碳战略
- Design tone: 高端咨询、深海蓝与活力绿，适合规划型汇报
- Theme mode: Light theme

## II. Canvas Specification

- Format: PPT 16:9
- ViewBox: `0 0 1280 720`
- Width: 1280
- Height: 720

## III. Color Scheme

- Primary: `#003F6C`
- Secondary: `#00A651`
- Accent: `#62B6CB`
- Background: `#F5FAFC`
- Surface: `#FFFFFF`
- Text: `#0F2D3F`

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
