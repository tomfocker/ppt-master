# PPT Master Fork

本仓库是 [hugohe3/ppt-master](https://github.com/hugohe3/ppt-master) 的 fork，保留原版“把 PDF / DOCX / URL / Markdown 生成原生可编辑 PPTX”的完整工作流，并在此基础上补充更适合中文使用和长期复用的模板资产。

> 原版项目由 Hugo He 创建并维护，采用 MIT License。本 fork 主要用于模板扩展、中文化索引和混合视觉模板实践。

中文 | [English](./README_EN.md)

---

## 当前同步状态

本 fork 已同步到上游 `upstream/main` 的 v2.6.0 时代能力，并保留我们自己的中文模板库扩展。

上游新增能力主要包括：

- PPTX 模板导入与复刻：可从现有 `.pptx` 提取 master、layout、assets 和可复用模板结构。
- 更强的 PPTX / SVG 往返保真：图片裁剪、主题背景、表格、占位符、嵌套 SVG、图片 transform 等能力增强。
- 新工作流：`topic-research`、`resume-execute`、`verify-charts`、`visual-edit`、`generate-audio`。
- 动画、转场、旁白、音频与视频导出相关文档与脚本增强。
- 示例库、在线预览索引和图标库扩展。

---

## 相对原版的升级

### 1. 中文优先的可复用模板库

本 fork 把一批高质量 `examples/` 项目抽象成可复用模板，放入：

```text
skills/ppt-master/templates/layouts/
```

这些模板不再绑定原始案例内容，而是保留其视觉语言、页面结构和设计节奏，适合直接在新 PPT 任务中点名使用。

新增的示例衍生模板包括：

| 模板 | 适合场景 |
|------|----------|
| `示例_项目介绍` | 产品介绍、项目路演、工具说明、内部宣讲 |
| `示例_暗色科技自动模式` | AI 安全、工程架构、研发分享 |
| `示例_像素风Git入门` | 技术培训、开发者入门课、游戏化知识分享 |
| `示例_易理风谦卦` | 传统文化研究、国学课程、哲学主题汇报 |
| `示例_禅意风金刚经` | 佛学讲座、经典研读、文化课程 |
| `示例_谷歌风年度报告` | 年度总结、团队复盘、项目盘点 |
| `示例_暗色代码调试` | 开发者培训、工程方法论、排障流程 |
| `示例_技术对比AI编程工具` | 工具评测、竞品分析、技术选型 |
| `示例_咨询风依恋心理` | 心理学课程、咨询培训、研究综述 |
| `示例_咨询风AI代理` | AI 架构、智能体设计、技术战略 |
| `示例_咨询风甘孜财政` | 财政分析、区域经济、政府汇报 |
| `示例_咨询风重庆区域` | 区域研究、财政金融、风险研判 |
| `示例_高端咨询南欧江` | 基础设施评估、能源项目、国际工程 |
| `示例_高端咨询汽车认证` | 五年规划、认证检测、汽车产业战略 |
| `示例_麦肯锡客户忠诚` | 客户研究、忠诚度分析、商业策略 |

### 2. 模板库扩展到 46 套

当前模板索引包含上游品牌风、政企风、通用商务风、学术/医疗/心理等场景模板，以及本 fork 新增的示例衍生模板和风格库模板。

完整索引：

- [模板说明](./skills/ppt-master/templates/layouts/README.md)
- [机器可读索引](./skills/ppt-master/templates/layouts/layouts_index.json)

### 3. 风格样片库与混合模板

本 fork 增加了一组 16:9 风格参考图，用于新模板设计、风格选择和视觉对齐。样片不是最终 PPT 页面，使用时应重建为可编辑 SVG / DrawingML 元素。

- [风格样片库](./skills/ppt-master/templates/style_samples/README.md)
- [样片索引](./skills/ppt-master/templates/style_samples/style_samples_index.json)

其中 10 个高频方向已经沉淀为可直接点名使用的 `layouts/` 模板：`风格_高端金融`、`风格_高端金融混合`、`风格_暗色AI工程`、`风格_暗色AI工程混合`、`风格_高端咨询`、`风格_高端咨询混合`、`风格_现代政企红`、`风格_现代政企红混合`、`风格_禅意经典`、`风格_能源基建`。

带“混合”的模板使用原生生图素材提供更强视觉质感，标题、卡片、指标、图表等信息层仍保持 SVG / DrawingML 可编辑。

---

## 使用方式

### 1. 安装依赖

需要 Python 3.10+。

```bash
pip install -r requirements.txt
```

Windows 用户可参考原版文档：

- [Windows 安装指南](./docs/zh/windows-installation.md)

### 2. 放入资料

建议把 PDF、DOCX、Markdown、图片等资料放到 `projects/` 目录下，例如：

```text
projects/my-report/sources/report.pdf
```

### 3. 在 AI Agent 里发起任务

使用本 fork 时，建议让 Agent 先读取 `AGENTS.md` 和 `skills/ppt-master/SKILL.md`，再开始生成。

普通自由设计：

```text
请读取 AGENTS.md 和 skills/ppt-master/SKILL.md，
然后用 projects/my-report/sources/report.pdf 生成一份 16:9 PPT。
```

指定本 fork 新增模板：

```text
请读取 AGENTS.md 和 skills/ppt-master/SKILL.md，
用「风格_暗色AI工程混合」模板，
根据 projects/ai-review/sources/report.pdf 生成一份 16:9 PPT。
```

指定示例衍生模板：

```text
请使用「示例_麦肯锡客户忠诚」模板生成咨询风 PPT。
```

> 模板是 opt-in 的：只有你明确点名模板时，工作流才会使用模板；否则默认自由设计。

### 4. 生成结果

生成完成后，导出的文件会保存到项目的 `exports/` 目录中，通常包含：

```text
*.pptx
*_svg.pptx
```

- `.pptx`：原生 PowerPoint 形状版本，可直接编辑
- `_svg.pptx`：视觉参考版本

---

## 常用命令

### 初始化项目

```bash
python3 skills/ppt-master/scripts/project_manager.py init my_deck --format ppt169
```

### 导入资料

```bash
python3 skills/ppt-master/scripts/project_manager.py import-sources projects/my_deck path/to/source.pdf --move
```

### 校验项目

```bash
python3 skills/ppt-master/scripts/project_manager.py validate projects/my_deck
```

### 后处理导出

以下命令必须按顺序单独执行，不要合并成一条命令：

```bash
python3 skills/ppt-master/scripts/total_md_split.py projects/my_deck
```

```bash
python3 skills/ppt-master/scripts/finalize_svg.py projects/my_deck
```

```bash
python3 skills/ppt-master/scripts/svg_to_pptx.py projects/my_deck -s final
```

---

## 与原版保持同步

本 fork 以原版为上游：

```text
upstream: https://github.com/hugohe3/ppt-master
origin:   https://github.com/tomfocker/ppt-master
```

如需同步上游：

```bash
git fetch upstream
git merge upstream/main
```

---

## 重要文档

| 文档 | 说明 |
|------|------|
| [AGENTS.md](./AGENTS.md) | 通用 AI Agent 入口说明 |
| [SKILL.md](./skills/ppt-master/SKILL.md) | PPT Master 完整工作流 |
| [模板库 README](./skills/ppt-master/templates/layouts/README.md) | 当前模板清单与模板结构 |
| [模板导入指南](./docs/zh/templates-guide.md) | 上游 v2.6 的 PPTX 模板复刻说明 |
| [音频旁白指南](./docs/zh/audio-narration.md) | 旁白、音频与视频导出 |
| [脚本说明](./skills/ppt-master/scripts/README.md) | 转换、项目管理、导出等工具 |
| [FAQ](./docs/zh/faq.md) | 常见问题 |

---

## License

本 fork 继承原项目的 MIT License。原项目版权和署名归原作者 Hugo He 及贡献者所有。
