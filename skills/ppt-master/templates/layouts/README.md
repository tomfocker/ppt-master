# Page Layout Template Library (43 Templates)

Pre-built PPT page layout templates supporting multiple styles and use cases.

- **Full Index**: [README.md](./README.md) (human browsing — includes categories, primary colors, detailed tone)
- **Slim Index**: [layouts_index.json](./layouts_index.json) (lightweight lookup — `label` / `summary` / `keywords` only)

> **Template selection is opt-in.** The main workflow defaults to free design and does NOT read `layouts_index.json` unless the user explicitly requests a template. See `SKILL.md` Step 3.

---

## Quick Template Index

| Template Name | Category | Use Cases | Primary Color | Design Tone |
|---------------|----------|-----------|---------------|-------------|
| `google_style` | Brand | Annual reports, tech sharing, data presentation | Google Four Colors `#4285F4` `#EA4335` `#FBBC04` `#34A853` | Modern clean, data-driven, ample whitespace |
| `mckinsey` | Brand | Strategic consulting, executive reports, investment analysis | McKinsey Blue `#005587` | Structured thinking, minimalist premium, MECE principle |
| `anthropic` | Brand | AI tech sharing, developer conferences, product launches | Anthropic Orange `#D97757` | Tech-forward, conclusion-first, dark cover |
| `china_telecom_template` | Brand | Telecom solutions, digital transformation plans,政企汇报 | Telecom Red `#C00000` | Restrained, authoritative, telecom enterprise style |
| `中汽研_常规` | Brand | Product certification, evaluation & testing | Deep Blue `#004098` | [Standard] Professional authority, consulting style |
| `中汽研_商务` | Brand | Business visits, technical exchanges | Blue Gradient `#003366` | [Business] Modern tech, composed and sophisticated |
| `中汽研_现代` | Brand | Strategic launches, future tech | Deep Blue `#001529` | [Future] Future Tech, neon glow |
| `中国电建_常规` | Brand | Power & energy, engineering, state-owned enterprise reports | PowerChina Blue `#00418D` | Craftsmanship, steady and reliable |
| `中国电建_现代` | Brand | International engineering, premium roadshows, tech innovation | Deep Sea Blue `#001F45` | [Modern] Grand narrative, digital tech |
| `招商银行` | Brand | Premium reports, VIP services, annual reports | CMB Red `#C41230` | Minimalist luxury, financial texture, borderless |
| `exhibit` | General | Exhibit-driven strategic reports, executive presentations, board briefings | Gradient top bar + Gold accents | Conclusion-first, data-driven, confidential |
| `academic_defense` | Scenario | Thesis defense, academic reports, grant proposals | Deep Blue + Red accents | Clear hierarchy, academic standards |
| `psychology_attachment` | Scenario | Psychotherapy training, counseling lectures | Blue-green gradient + Colorful semantic colors | Warm professional, therapeutic feel |
| `medical_university` | Scenario | Medical reports, case discussions, research presentations | Medical Blue `#0066B3` | Professional rigorous, life-affirming |
| `government_red` | Government/Enterprise | Government work reports, party-building presentations | Government Red `#8B0000` | Solemn authority, grand and imposing |
| `government_blue` | Government/Enterprise | Smart cities, open governance, digital transformation | Tech Blue `#0050B3` | Modern tech, rigorous and rational |
| `ai_ops` | Government/Enterprise | Telecom AI ops, IT system overview, digital intelligence solutions | Telecom Red `#C00000` + Blue `#2E75B6` | High information density, modular layout, telecom style |
| `pixel_retro` | Special | Git/tech introductions, retro gaming themes | Neon colors `#00FF41` `#FF0080` | Pixel art, cyberpunk |
| `科技蓝商务` | General | Corporate reports, product launches, proposals | Tech Blue `#0078D7` | Tech, business, professional, clean |
| `smart_red` | General | Tech company profiles, education solutions | Smart Red-Orange `#DE3545` | Modern, vibrant, geometric |
| `重庆大学` | Scenario | Academic defense, research presentations | CQU Blue `#006BB7` | Academic solidity, mountain-city character |
| `示例_项目介绍` | Example-derived | 产品介绍、项目路演、工具说明、内部宣讲 | #2563EB | 清晰、现代、结构化，强调功能模块与价值递进 |
| `示例_暗色科技自动模式` | Example-derived | AI 安全、工程架构、技术复盘、研发分享 | #60A5FA | 深色、克制、工程化，带有安全评审和系统架构气质 |
| `示例_像素风Git入门` | Example-derived | 技术培训、开发者入门课、游戏化知识分享 | #00FF41 | 像素复古、轻松、鲜明，适合降低技术主题的距离感 |
| `示例_易理风谦卦` | Example-derived | 传统文化研究、国学课程、哲学主题汇报、文化讲座 | #8B5A2B | 古朴、沉静、象数结构感，强调层层递进的学术叙述 |
| `示例_禅意风金刚经` | Example-derived | 佛学讲座、经典研读、文化课程、哲学分享 | #6B7A5A | 留白、宁静、东方美学，适合慢节奏的文本阐释 |
| `示例_谷歌风年度报告` | Example-derived | 年度总结、技术成果汇报、团队复盘、项目盘点 | #4285F4 | 明快、干净、数据友好，以四色点缀建立节奏 |
| `示例_暗色代码调试` | Example-derived | 开发者培训、工程方法论、排障流程、内部技术分享 | #58A6FF | 暗色代码、流程清晰、适合步骤化方法讲解 |
| `示例_技术对比AI编程工具` | Example-derived | 工具评测、竞品分析、技术选型、横向对比 | #2563EB | 清爽、评测导向、强调对比维度和结论 |
| `示例_咨询风依恋心理` | Example-derived | 心理学课程、咨询培训、临床理论汇报、研究综述 | #1E3A5F | 专业、温和、咨询式结构，兼顾治疗主题的人文温度 |
| `示例_咨询风AI代理` | Example-derived | AI 架构、智能体设计、技术战略、开发者分享 | #D97757 | 咨询式结论先行，带 Anthropic 风格的暖橙科技感 |
| `示例_咨询风甘孜财政` | Example-derived | 财政分析、区域经济、政府汇报、投融资研究 | #1E3A5F | 稳健、正式、数据密集，带区域文化色彩的政府咨询风 |
| `示例_咨询风重庆区域` | Example-derived | 区域研究、财政金融、城投分析、风险研判 | #1E3A5F | 专业金融研究、结构化、适合复杂指标与表格呈现 |
| `示例_高端咨询南欧江` | Example-derived | 基础设施评估、能源项目、国际工程、风险战略汇报 | #003F6C | 高端咨询、深水蓝调、具有危机评估和战略判断张力 |
| `示例_高端咨询汽车认证` | Example-derived | 五年规划、认证检测、汽车产业、绿色低碳战略 | #003F6C | 高端咨询、深海蓝与活力绿，适合规划型汇报 |
| `示例_麦肯锡客户忠诚` | Example-derived | 客户研究、忠诚度分析、经营诊断、商业策略汇报 | #005587 | 经典咨询、MECE、极简数据驱动，强调结论与图表 |
| `premium_finance` | Style Library | 银行、财富管理、交易银行、金融高管汇报 | #8B1020 | 高端金融、温润留白、红金点缀，适合产品方案与经营汇报 |
| `dark_ai_engineering` | Style Library | AI 安全、工程架构、系统评审、开发者分享 | #58A6FF | 深色工程界面、系统图、风险矩阵，适合技术深潜 |
| `dark_ai_engineering_hybrid` | Style Library | AI 安全、工程架构、技术深潜、研发复盘 | #58A6FF | 生图背景质感 + 可编辑信息层，适合观感优先的技术汇报 |
| `consulting_executive` | Style Library | 董事会汇报、战略咨询、投资分析、市场研究 | #005587 | 高端咨询、强网格、结论先行，强调数据和决策层阅读 |
| `government_red_modern` | Style Library | 政府报告、国企汇报、政策沟通、年度总结 | #9B111E | 现代政企红、正式稳重、象征性克制 |
| `zen_classics` | Style Library | 经典研读、哲学课程、传统文化、人文讲座 | #4F5B45 | 宣纸留白、东方水墨、沉静克制，适合慢节奏阐释 |
| `energy_infrastructure` | Style Library | 能源基建、国际工程、投资评估、风险战略 | #003F6C | 深海蓝咨询风、项目地图、风险矩阵、工程战略感 |
---

## Template Categories

### 1. Brand Style Templates

Templates mimicking **specific well-known brands/institutions** with their exclusive design style.
> **Characteristics**: Distinctive brand identity (specific logos, color schemes, VI standards), suitable for internal or external presentations of that organization. Examples: Google, McKinsey, PowerChina.

| Template | Description |
|----------|-------------|
| `google_style` | Google Material Design style, four-color brand identity |
| `mckinsey` | McKinsey consulting style, data-driven and structured |
| `anthropic` | Anthropic AI style, dark tech-forward aesthetic |
| `china_telecom_template` | China Telecom brand style, red-gray structural header + ribbon footer |
| `中汽研_常规` | CATARC standard style (v1), suitable for certification and evaluation |
| `中汽研_商务` | CATARC business style (v2), modern tech business, composed and sophisticated |
| `中汽研_现代` | CATARC modern style (v3 Future), Future Tech style, deep blue + neon cyan |
| `中国电建_常规` | PowerChina standard style (v1), suitable for power, energy, and engineering SOEs |
| `中国电建_现代` | PowerChina modern style (v2), emphasis on grand narrative and digital tech |
| `招商银行` | China Merchants Bank v2.0, minimalist luxury, borderless open layout |

### 2. General Style Templates

Universal business styles not tied to any specific brand, broadly applicable.

| Template | Description |
|----------|-------------|
| `exhibit` | Exhibit-driven style, conclusion-first layout with Exhibit takeaway bar, gradient top bar, grid decoration |
| `consulting_executive` | High-end executive consulting style for strategy decks, board reports, and investment analysis |
| `premium_finance` | Premium banking and finance style for wealth management and transaction banking reports |
| `energy_infrastructure` | Deep-blue infrastructure consulting style for energy projects and international engineering |
| `科技蓝商务` | Tech business style, rigorous and professional, hexagonal texture |
| `smart_red` | Smart red-orange business style, modern and vibrant, geometric cutaway design |

### 3. Scenario-Specific Templates

Designed for **specific use cases**, with content structures tailored to scenario requirements.

| Template | Description |
|----------|-------------|
| `academic_defense` | Academic defense, clear research content hierarchy |
| `psychology_attachment` | Psychotherapy theme, warm and professional color palette |
| `medical_university` | Hospital / medical university template, suitable for medical reports |
| `重庆大学` | Chongqing University template, blending mountain-city layered imagery with modern academic style |

### 4. Government & Enterprise Templates

Industry-standard designs for **government agencies and general state-owned enterprises**.
> **Distinction**: Unlike brand styles, these are not targeted at specific organizations but provide templates matching the common aesthetic preferences of government/SOE contexts (e.g., official document red, smart governance blue).

| Template | Description |
|----------|-------------|
| `government_red` | Red government style, suitable for government work reports, party-building events |
| `government_red_modern` | Modernized formal red style for government reports, SOE briefings, and policy communication |
| `government_blue` | Blue government style, suitable for smart cities, digital governance reports |
| `ai_ops` | Enterprise digital intelligence style, telecom AI ops architecture, high-density reports (includes `reference_style.svg` style reference) |

### 5. Special Style Templates

Unconventional visual styles for specific creative scenarios.

| Template | Description |
|----------|-------------|
| `pixel_retro` | Pixel retro style, cyberpunk / gaming themes |
| `dark_ai_engineering` | Dark technical interface style for AI engineering, architecture, and system-review decks |
| `zen_classics` | Ink-wash and paper-texture style for traditional culture, philosophy, and classical text study |

### 6. Style Library Templates

Reusable style packages converted from the `style_samples/` visual direction boards into editable SVG page skeletons. These are template-library assets, not screenshot references.

| Template | Description |
|----------|-------------|
| `premium_finance` | Premium finance and banking report style with red, pearl white, graphite, and gold accents. |
| `dark_ai_engineering` | Dark AI engineering style with technical panels, architecture-review rhythm, and cyan/blue accents. |
| `dark_ai_engineering_hybrid` | Hybrid AI engineering style using raster-generated atmospheric backgrounds with editable SVG text, cards, and charts. |
| `consulting_executive` | Executive consulting style with deep navy grid discipline and board-report hierarchy. |
| `government_red_modern` | Modern formal red style for government and SOE reporting. |
| `zen_classics` | Zen-inspired cultural lecture style with warm paper, ink, moss green, and cinnabar accents. |
| `energy_infrastructure` | Energy infrastructure consulting style for project maps, risk matrices, and investment review decks. |

### 7. Example-Derived Templates

Reusable layout templates abstracted from curated `examples/` projects. These packages preserve the source examples' visual language while replacing project-specific copy, data, and slide content with standard placeholders.

| Template | Description |
|----------|-------------|
| `示例_项目介绍` | 从 PPT Master 项目介绍案例抽象出的通用产品/项目介绍模板。 |
| `示例_暗色科技自动模式` | 从 Claude Code Auto Mode 案例抽象出的暗色 AI 安全/工程深潜模板。 |
| `示例_像素风Git入门` | 从 Git 入门像素风案例抽象出的复古技术教学模板。 |
| `示例_易理风谦卦` | 从地山谦卦研究案例抽象出的东方哲思与传统文化研究模板。 |
| `示例_禅意风金刚经` | 从金刚经研究案例抽象出的禅意留白与经典研读模板。 |
| `示例_谷歌风年度报告` | 从 Google 年度报告案例抽象出的轻量品牌色年度总结模板。 |
| `示例_暗色代码调试` | 从 Debug 六步法案例抽象出的代码培训与方法论模板。 |
| `示例_技术对比AI编程工具` | 从三大 AI 编程工具横向对比案例抽象出的技术评测模板。 |
| `示例_咨询风依恋心理` | 从心理治疗中的依恋案例抽象出的咨询式心理学课程模板。 |
| `示例_咨询风AI代理` | 从构建有效 AI 代理案例抽象出的 AI 架构与技术策略模板。 |
| `示例_咨询风甘孜财政` | 从甘孜州经济财政分析案例抽象出的政府财政与区域分析模板。 |
| `示例_咨询风重庆区域` | 从重庆市区域报告案例抽象出的区域金融研究与风险分析模板。 |
| `示例_高端咨询南欧江` | 从南欧江水电站战略评估案例抽象出的重大工程战略评估模板。 |
| `示例_高端咨询汽车认证` | 从汽车认证五年战略规划案例抽象出的认证机构战略规划模板。 |
| `示例_麦肯锡客户忠诚` | 从客户忠诚度分析案例抽象出的经典麦肯锡式咨询模板。 |

> **Design philosophy**: Style and scenario are **orthogonal** concepts. Scenario templates define content structure; style templates define visual presentation. In theory, scenario templates can be combined with different styles.

---

## Template File Structure

Each template should contain the following standard files (TOC page is optional):

| Filename | Required | Purpose | Description |
|----------|----------|---------|-------------|
| `design_spec.md` | Yes | Design specification | Complete color, typography, and layout specs |
| `01_cover.svg` | Yes | Cover page | Title, subtitle, date, organization |
| `02_toc.svg` | Optional | Table of contents | Chapter list, navigation |
| `02_chapter.svg` | Yes | Chapter page | Chapter number, chapter title |
| `03_content.svg` | Yes | Content page | Fixed header/footer, flexible content area |
| `04_ending.svg` | Yes | Ending page | Thank-you message, contact info |

> **Design philosophy**: Templates define visual consistency and structural pages; content pages maintain maximum flexibility, letting AI determine layout based on actual content.

---

## design_spec.md Standard Structure

All template design specification documents should follow this chapter structure:

```markdown
# [Template Name] - Design Specification

> One-line description of applicable scenarios

## I. Template Overview
## II. Canvas Specification
## III. Color Scheme
## IV. Typography System
## V. Page Structure
## VI. Page Types
## VII. Layout Modes (Recommended)
## VIII. Spacing Specification
## IX. SVG Technical Constraints
## X. Placeholder Specification
## XI. Usage Guide (Recommended)
```

---

## Placeholder Specification

Templates use `{{PLACEHOLDER}}` format to mark replaceable content:

> For **newly created library templates**, use the canonical placeholder contract below. Some existing templates still contain legacy placeholder variants; those should be treated as historical exceptions rather than the standard for new assets.

### General Placeholders

| Placeholder | Purpose | Applicable Pages |
|-------------|---------|-----------------|
| `{{TITLE}}` | Main title | Cover |
| `{{SUBTITLE}}` | Subtitle | Cover |
| `{{DATE}}` | Date | Cover, Ending |
| `{{AUTHOR}}` | Author / Organization (Chinese) | Cover |
| `{{AUTHOR_EN}}` | Author / Organization (English) | Cover |

### Chapter-Related

| Placeholder | Purpose | Applicable Pages |
|-------------|---------|-----------------|
| `{{CHAPTER_NUM}}` | Chapter number | Chapter, Content |
| `{{CHAPTER_TITLE}}` | Chapter title | Chapter |
| `{{CHAPTER_TITLE_EN}}` | Chapter English subtitle | Chapter |

### Content Page

| Placeholder | Purpose | Applicable Pages |
|-------------|---------|-----------------|
| `{{PAGE_TITLE}}` | Page title | Content |
| `{{CONTENT_AREA}}` | Content area placeholder | Content |
| `{{PAGE_NUM}}` | Page number | Content, Ending |
| `{{SOURCE}}` | Data source | Content footer |

### Table of Contents

| Placeholder | Purpose |
|-------------|---------|
| `{{TOC_ITEM_1_TITLE}}` ~ `{{TOC_ITEM_N_TITLE}}` | TOC item titles |
| `{{TOC_ITEM_1_DESC}}` ~ `{{TOC_ITEM_N_DESC}}` | Optional TOC item descriptions |
| `{{TOC_ITEM_1}}` ~ `{{TOC_ITEM_N}}` | Legacy simple TOC items; do not use for new templates unless no description field is needed |

### Ending Page

| Placeholder | Purpose |
|-------------|---------|
| `{{THANK_YOU}}` | Thank-you message |
| `{{ENDING_SUBTITLE}}` | Ending page subtitle |
| `{{CLOSING_MESSAGE}}` | Closing message |
| `{{CONTACT_INFO}}` | Contact information |

---

## Usage

### Copy from Template Library to Project

```bash
# Copy exhibit style template to project
cp templates/layouts/exhibit/* projects/<project>/templates/

# Copy Google style template to project
cp templates/layouts/google_style/* projects/<project>/templates/

# Copy government style template to project (e.g., government red)
cp templates/layouts/government_red/* projects/<project>/templates/
```

### After Copying

1. Read `design_spec.md` to understand the design specification
2. Adjust colors based on project requirements (if needed)
3. Place logo files in the `images/` directory
4. Use the Executor role to generate SVG pages based on templates

---

## Template Development Guide

### Creating New Templates

1. Create a new directory under `templates/layouts/`
2. Create required files following the existing template structure
3. Ensure `design_spec.md` follows the standard chapter structure
4. All SVGs use `viewBox="0 0 1280 720"`
5. Follow SVG technical constraints (see below)
6. Validate the template directory with `python3 scripts/svg_quality_checker.py templates/layouts/<template_name> --format ppt169`
7. Register the new template in `templates/layouts/layouts_index.json` with three fields: `label`, `summary`, `keywords`

`layouts_index.json` is the lightweight lookup used when a user explicitly opts into the template flow. A template folder without an index entry will not be discoverable by that flow.

### SVG Technical Constraints (All Templates Must Comply)

#### Required

- viewBox: `0 0 1280 720`
- Backgrounds use `<rect>` elements
- Text wrapping uses `<tspan>`
- Transparency uses `fill-opacity` / `stroke-opacity`
- Gradients use `<defs>` with `<linearGradient>`

#### Forbidden (PPT Incompatible)

| Banned Element | Alternative |
|----------------|-------------|
| `<foreignObject>` | Use `<text>` + `<tspan>` |
| `clipPath` on shapes / groups / text | Draw the target geometry directly with the matching native element (`<circle>` / `<ellipse>` / `<rect rx>` / `<polygon>` / `<path>`). `clipPath` on `<image>` elements is conditionally allowed — see shared-standards.md §1.2 |
| `mask` | Use `fill-opacity` |
| `<style>` / `class` | Use inline styles |
| `textPath` | Use plain `<text>` |
| `animate*` | Static design |
| `script` | No interactivity supported |
| `rgba()` | Use HEX + `fill-opacity` |
| `<g opacity="...">` | Set opacity on each child element individually |

---
