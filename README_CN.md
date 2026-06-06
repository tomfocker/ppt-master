# PPT Master Fork

[![Version](https://img.shields.io/badge/version-v2.9.0-blue.svg)](https://github.com/hugohe3/ppt-master/releases)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

中文 | [English](./README_EN.md)

本仓库是 [hugohe3/ppt-master](https://github.com/hugohe3/ppt-master) 的 fork。原项目是一套 AI 驱动的 PPT 生成工作流：把 PDF、DOCX、网页、Markdown 或现有 PPTX 资料转换成原生可编辑的 PowerPoint 文件。

本 fork 的重点不是另起炉灶，而是在跟随上游能力的基础上，沉淀更适合中文使用和复用的模板资产：中文可读的模板索引、示例衍生模板、风格样片库，以及“生图背景 + 可编辑信息层”的混合模板。

> 原项目由 Hugo He 创建并维护，采用 MIT License。本 fork 保留原项目署名和许可边界，主要用于模板扩展、中文化索引和长期可复用风格库实践。

---

## 当前同步状态

本 fork 已整合上游 `main` 的 v2.9.0 时代更新，同时保留我们自己的模板库和样片库。

已经同步进来的上游能力包括：

- 直接 PPTX 套模板路线：通过 [`template-fill-pptx`](./skills/ppt-master/workflows/template-fill-pptx.md) 复用现有 PPTX 页面并回填新内容。
- 三类模板架构：`brands/` 管身份，`layouts/` 管结构，`decks/` 管整套 PPT 复刻。
- Live Preview 与直接编辑：浏览器里点选元素、改文字/样式、拖拽移动、方向键微调，再写回 `svg_output/`。
- 视觉自检工作流：[`visual-review`](./skills/ppt-master/workflows/visual-review.md) 可按 rubric 逐页检查 SVG 观感。
- LaTeX 公式渲染、图表数据校准、自动动画、旁白音频和视频导出能力增强。
- 71 个可视化模板、11,600+ 图标资源，以及一批新的官方示例 deck。

---

## 相对原版的升级

### 1. 中文优先的复用入口

我们把 fork 的入口说明改成中文优先，并把常用模板、样片和使用方式写在根 README 中。以后让 Agent 进入这个仓库时，先读 [`AGENTS.md`](./AGENTS.md) 和 [`skills/ppt-master/SKILL.md`](./skills/ppt-master/SKILL.md)，再执行 PPT 任务。

### 2. 可复用模板资产库

当前模板资产按上游 v2.9 架构拆成三类：

| 类型 | 目录 | 用途 | 数量 |
|------|------|------|-----:|
| Brand | [`templates/brands/`](./skills/ppt-master/templates/brands/) | 只锁定品牌身份，如颜色、字体、logo、语气 | 2 |
| Layout | [`templates/layouts/`](./skills/ppt-master/templates/layouts/) | 只锁定页面结构和 SVG 页面骨架 | 32 |
| Deck | [`templates/decks/`](./skills/ppt-master/templates/decks/) | 复刻完整 PPT 风格，包含身份和结构 | 8 |

常用的 fork 模板包括：

| 模板路径 | 适合场景 |
|----------|----------|
| `skills/ppt-master/templates/layouts/风格_暗色AI工程混合/` | AI 工程、安全评审、系统架构、技术复盘 |
| `skills/ppt-master/templates/layouts/风格_高端金融混合/` | 银行、财富管理、交易银行、金融高管汇报 |
| `skills/ppt-master/templates/layouts/风格_高端咨询混合/` | 董事会汇报、战略咨询、投资分析、研究报告 |
| `skills/ppt-master/templates/layouts/风格_现代政企红混合/` | 政府报告、国企汇报、政策沟通、年度总结 |
| `skills/ppt-master/templates/layouts/示例_麦肯锡客户忠诚/` | 客户研究、忠诚度分析、商业策略 |
| `skills/ppt-master/templates/decks/招商银行/` | 交易银行产品介绍、销售收款方案、客户案例拆解 |

注意：模板触发必须给出完整目录路径。裸模板名只适合查询和讨论，不会自动进入模板流程。

### 3. 风格样片库

[`templates/style_samples/`](./skills/ppt-master/templates/style_samples/) 保存了一组 16:9 风格参考图，用来做新模板设计、风格对齐和提示词参考。样片不是最终 PPT 页面，真正生成 deck 时仍应重建为可编辑 SVG / DrawingML 元素。

样片库目前覆盖高端咨询、现代政企红、暗色 AI 工程、学术研究、医学高校、高端金融、科技年度报告、心理咨询、像素技术培训、禅意经典、能源基建、汽车认证等方向。

### 4. 混合模板路线

我们保留并扩展了“混合模板”方案：背景用原生生图素材承担高级视觉质感，标题、卡片、指标、图表、流程线和正文保持 SVG / DrawingML 可编辑。

这条路线比纯 SVG 更接近原生 AI 生成 PPT 的观感，同时比整页图片更方便后期改文字和数据，是目前比较值得继续积累的方向。

---

## 使用方式

### 1. 安装依赖

需要 Python 3.10+。

```bash
pip install -r requirements.txt
```

Windows 用户参考：[`docs/zh/windows-installation.md`](./docs/zh/windows-installation.md)。

### 2. 放入资料

建议把资料放在 `projects/<项目名>/sources/` 下，例如：

```text
projects/my-report/sources/report.pdf
```

也可以使用 DOCX、XLSX、PPTX、Markdown、网页 URL 或直接粘贴主题。

### 3. 让 Agent 读取工作流

普通自由设计：

```text
请读取 AGENTS.md 和 skills/ppt-master/SKILL.md，
用 projects/my-report/sources/report.pdf 生成一份 16:9 PPT。
```

指定 fork 模板：

```text
请读取 AGENTS.md 和 skills/ppt-master/SKILL.md，
使用模板路径 skills/ppt-master/templates/layouts/风格_暗色AI工程混合/，
根据 projects/ai-review/sources/report.pdf 生成一份 16:9 PPT。
```

使用整套 deck 复刻模板：

```text
请使用模板路径 skills/ppt-master/templates/decks/招商银行/，
把 projects/bank-plan/sources/方案.md 做成一份交易银行产品介绍 PPT。
```

使用现有 PPTX 套模板：

```text
请读取 skills/ppt-master/workflows/template-fill-pptx.md，
用 projects/template/source.pptx 作为模板，
把 projects/new-content/sources/content.md 填成一份新 PPT。
```

### 4. 常用命令

初始化项目：

```bash
python3 skills/ppt-master/scripts/project_manager.py init my_deck --format ppt169
```

导入资料：

```bash
python3 skills/ppt-master/scripts/project_manager.py import-sources projects/my_deck path/to/source.pdf --move
```

校验项目：

```bash
python3 skills/ppt-master/scripts/project_manager.py validate projects/my_deck
```

后处理导出，必须一条一条顺序执行：

```bash
python3 skills/ppt-master/scripts/total_md_split.py projects/my_deck
```

```bash
python3 skills/ppt-master/scripts/finalize_svg.py projects/my_deck
```

```bash
python3 skills/ppt-master/scripts/svg_to_pptx.py projects/my_deck
```

默认导出原生可编辑 PPTX；需要额外生成 SVG 快照版时加 `--svg-snapshot`。

---

## 目录速查

| 路径 | 说明 |
|------|------|
| [`AGENTS.md`](./AGENTS.md) | AI Agent 入口规则 |
| [`skills/ppt-master/SKILL.md`](./skills/ppt-master/SKILL.md) | PPT Master 主工作流 |
| [`skills/ppt-master/workflows/`](./skills/ppt-master/workflows/) | 主题研究、模板创建、套模板、预览、视觉自检、音频等子工作流 |
| [`skills/ppt-master/templates/`](./skills/ppt-master/templates/) | 模板、样片、图表、图标资源 |
| [`examples/`](./examples/) | 示例项目和模板预览样片 |
| [`projects/`](./projects/) | 本地生成项目工作区 |

---

## 与上游同步

本仓库远端关系：

```text
upstream: https://github.com/hugohe3/ppt-master
origin:   https://github.com/tomfocker/ppt-master
```

同步上游：

```bash
git fetch upstream
git merge upstream/main
```

同步后需要重点检查 README、模板索引和示例索引，确保 fork 的中文模板资产仍然可发现。

---

## License

本 fork 继承原项目 MIT License。原项目版权和署名归 Hugo He 及贡献者所有。
