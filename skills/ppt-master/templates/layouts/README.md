# Layout Templates

Layout 是“结构模板”：锁定画布、页面骨架、页面类型和 SVG 页面清单，但不强制品牌色、logo、字体语气等身份元素。身份可以来自 `templates/brands/`，完整机构风格复刻则放在 `templates/decks/`。

数据模型说明见 [`docs/zh/templates-architecture.md`](../../../../docs/zh/templates-architecture.md)。机器可读索引见 [`layouts_index.json`](./layouts_index.json)。

## 触发规则

模板选择必须显式给出目录路径，例如 `skills/ppt-master/templates/layouts/风格_暗色AI工程混合/`。只说模板名或只让 AI 浏览索引，不会自动进入模板流程。详见 [`SKILL.md`](../../SKILL.md) Step 3。

## 当前 Layout 清单

| ID | 中文说明 | 页数 | 适合场景 | 路径 |
|----|----------|----:|----------|------|
| `academic_defense` | 学术答辩 | 5 | 学位答辩、学术汇报、科研进展、基金申请。 | `skills/ppt-master/templates/layouts/academic_defense/` |
| `ai_ops` | AI 运维架构 | 6 | 电信 AI 运维架构、IT 系统总览、数智化方案、智慧基础设施汇报。 | `skills/ppt-master/templates/layouts/ai_ops/` |
| `government_blue` | 政企蓝 | 5 | 重点项目汇报、五年规划、工作总结、招商推介、政策解读。 | `skills/ppt-master/templates/layouts/government_blue/` |
| `government_red` | 政企红 | 5 | 政府汇报、政策解读、工作总结、项目介绍、招商推介。 | `skills/ppt-master/templates/layouts/government_red/` |
| `medical_university` | 医学高校 | 5 | 医学学术汇报、病例讨论、科研展示、医院工作报告、医学教育培训。 | `skills/ppt-master/templates/layouts/medical_university/` |
| `pixel_retro` | 像素复古 | 5 | 技术分享、编程教程、游戏化课程、极客风展示。 | `skills/ppt-master/templates/layouts/pixel_retro/` |
| `psychology_attachment` | 依恋心理 | 5 | 心理治疗培训、学术讲座、咨询案例分析、专业分享。 | `skills/ppt-master/templates/layouts/psychology_attachment/` |
| `示例_项目介绍` | 项目介绍示例模板 | 5 | 从 PPT Master 项目介绍案例抽象出的通用产品/项目介绍模板。 | `skills/ppt-master/templates/layouts/示例_项目介绍/` |
| `示例_暗色科技自动模式` | 暗色科技自动模式示例模板 | 5 | 从 Claude Code Auto Mode 案例抽象出的暗色 AI 安全/工程深潜模板。 | `skills/ppt-master/templates/layouts/示例_暗色科技自动模式/` |
| `示例_像素风Git入门` | 像素风 Git 入门示例模板 | 5 | 从 Git 入门像素风案例抽象出的复古技术教学模板。 | `skills/ppt-master/templates/layouts/示例_像素风Git入门/` |
| `示例_易理风谦卦` | 易理风谦卦示例模板 | 5 | 从地山谦卦研究案例抽象出的东方哲思与传统文化研究模板。 | `skills/ppt-master/templates/layouts/示例_易理风谦卦/` |
| `示例_禅意风金刚经` | 禅意风金刚经示例模板 | 5 | 从金刚经研究案例抽象出的禅意留白与经典研读模板。 | `skills/ppt-master/templates/layouts/示例_禅意风金刚经/` |
| `示例_谷歌风年度报告` | 谷歌风年度报告示例模板 | 5 | 从 Google 年度报告案例抽象出的轻量品牌色年度总结模板。 | `skills/ppt-master/templates/layouts/示例_谷歌风年度报告/` |
| `示例_暗色代码调试` | 暗色代码调试示例模板 | 5 | 从 Debug 六步法案例抽象出的代码培训与方法论模板。 | `skills/ppt-master/templates/layouts/示例_暗色代码调试/` |
| `示例_技术对比AI编程工具` | 技术对比 AI 编程工具示例模板 | 5 | 从三大 AI 编程工具横向对比案例抽象出的技术评测模板。 | `skills/ppt-master/templates/layouts/示例_技术对比AI编程工具/` |
| `示例_咨询风依恋心理` | 咨询风依恋心理示例模板 | 5 | 从心理治疗中的依恋案例抽象出的咨询式心理学课程模板。 | `skills/ppt-master/templates/layouts/示例_咨询风依恋心理/` |
| `示例_咨询风AI代理` | 咨询风 AI 代理示例模板 | 5 | 从构建有效 AI 代理案例抽象出的 AI 架构与技术策略模板。 | `skills/ppt-master/templates/layouts/示例_咨询风AI代理/` |
| `示例_咨询风甘孜财政` | 咨询风甘孜财政示例模板 | 5 | 从甘孜州经济财政分析案例抽象出的政府财政与区域分析模板。 | `skills/ppt-master/templates/layouts/示例_咨询风甘孜财政/` |
| `示例_咨询风重庆区域` | 咨询风重庆区域示例模板 | 5 | 从重庆市区域报告案例抽象出的区域金融研究与风险分析模板。 | `skills/ppt-master/templates/layouts/示例_咨询风重庆区域/` |
| `示例_高端咨询南欧江` | 高端咨询南欧江示例模板 | 5 | 从南欧江水电站战略评估案例抽象出的重大工程战略评估模板。 | `skills/ppt-master/templates/layouts/示例_高端咨询南欧江/` |
| `示例_高端咨询汽车认证` | 高端咨询汽车认证示例模板 | 5 | 从汽车认证五年战略规划案例抽象出的认证机构战略规划模板。 | `skills/ppt-master/templates/layouts/示例_高端咨询汽车认证/` |
| `示例_麦肯锡客户忠诚` | 麦肯锡客户忠诚示例模板 | 5 | 从客户忠诚度分析案例抽象出的经典麦肯锡式咨询模板。 | `skills/ppt-master/templates/layouts/示例_麦肯锡客户忠诚/` |
| `风格_高端金融` | 高端金融风格模板 | 5 | Premium banking and finance template for wealth management, transaction banking, and executive finance reports. | `skills/ppt-master/templates/layouts/风格_高端金融/` |
| `风格_暗色AI工程` | 暗色 AI 工程风格模板 | 5 | Dark technical template for AI safety, architecture reviews, system design, and developer presentations. | `skills/ppt-master/templates/layouts/风格_暗色AI工程/` |
| `风格_高端咨询` | 高端咨询风格模板 | 5 | High-end executive consulting template for board reports, strategy decks, and investment analysis. | `skills/ppt-master/templates/layouts/风格_高端咨询/` |
| `风格_现代政企红` | 现代政企红风格模板 | 5 | Modern formal red template for government reports, SOE briefings, and policy-oriented presentations. | `skills/ppt-master/templates/layouts/风格_现代政企红/` |
| `风格_禅意经典` | 禅意经典风格模板 | 5 | Ink-wash and paper-texture inspired template for classical text study, philosophy, and traditional culture lectures. | `skills/ppt-master/templates/layouts/风格_禅意经典/` |
| `风格_能源基建` | 能源基建风格模板 | 5 | Deep-blue infrastructure consulting template for energy projects, international engineering, and investment reviews. | `skills/ppt-master/templates/layouts/风格_能源基建/` |
| `风格_暗色AI工程混合` | 暗色 AI 工程混合风格模板 | 5 | Hybrid visual template for AI safety, architecture reviews, and engineering deep dives, using raster atmosphere backgrounds plus editable SVG information layers. | `skills/ppt-master/templates/layouts/风格_暗色AI工程混合/` |
| `风格_高端金融混合` | 高端金融混合风格模板 | 5 | Hybrid visual template for private banking, wealth management, transaction finance, and executive finance reports. | `skills/ppt-master/templates/layouts/风格_高端金融混合/` |
| `风格_高端咨询混合` | 高端咨询混合风格模板 | 5 | Hybrid visual template for board reports, strategy consulting, investment analysis, and executive decision decks. | `skills/ppt-master/templates/layouts/风格_高端咨询混合/` |
| `风格_现代政企红混合` | 现代政企红混合风格模板 | 5 | Hybrid visual template for government reports, SOE briefings, policy communication, and formal annual summaries. | `skills/ppt-master/templates/layouts/风格_现代政企红混合/` |


## design_spec.md schema

Layout 只写结构段。不要在 layout 的 `design_spec.md` 中写品牌身份段，例如 Color Scheme、Typography、Logo、Voice、Icon Style 的硬锁定；这些属于 `templates/brands/` 或 `templates/decks/`。

推荐 frontmatter：

```yaml
---
layout_id: <slug>
kind: layout
summary: <one-line use cases>
canvas_format: ppt169
page_count: 5
page_types: [cover, toc, chapter, content, ending]
---
```

推荐正文结构：

```markdown
# [Template Name] - Design Specification

## I. Template Overview
## II. Canvas Specification
## III. Page Structure
## IV. Page Types
## V. SVG Page Roster
```

## 标准文件集合

| 文件 | 是否必需 | 用途 |
|------|----------|------|
| `design_spec.md` | 是 | 模板结构说明 |
| `01_cover.svg` | 是 | 封面页 |
| `02_toc.svg` | 可选 | 目录页 |
| `02_chapter.svg` | 是 | 章节页 |
| `03_content.svg` | 是 | 内容页 |
| `04_ending.svg` | 是 | 结束页 |

所有 SVG 使用 `viewBox="0 0 1280 720"`。

## 占位符约定

- 使用清晰的 `{{PLACEHOLDER_NAME}}`，例如 `{{TITLE}}`、`{{PAGE_TITLE}}`、`{{CONTENT_AREA}}`。
- 占位符只表达内容角色，不写真实项目文案。
- 复杂页面可以在 SVG 中保留结构化模块，但文本和数字应可替换。

## 创建新 Layout

1. 在 `skills/ppt-master/templates/layouts/<id>/` 下创建目录。
2. 放入 `design_spec.md` 和标准 SVG 页面。
3. 确保 SVG 符合 [`references/shared-standards.md`](../../references/shared-standards.md)。
4. 校验模板：

```bash
python3 skills/ppt-master/scripts/svg_quality_checker.py skills/ppt-master/templates/layouts/<id> --template-mode --format ppt169
```

5. 注册索引：

```bash
python3 skills/ppt-master/scripts/register_template.py <id> --kind layout
```

## See also

- [`templates/brands/`](../brands/)：身份预设。
- [`templates/decks/`](../decks/)：完整 deck 复刻。
- [`templates/style_samples/`](../style_samples/)：风格参考样片。
