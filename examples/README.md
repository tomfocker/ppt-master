# 示例项目

> 这个目录保存 PPT Master 的示例项目，并由 [`examples.json`](./examples.json) 驱动在线预览和项目索引。

本 fork 在上游示例库之外，额外保留了两个模板预览样片：

- `template_preview_dark_ai_engineering_ppt169_20260508`：纯 SVG 可编辑的暗色 AI 工程模板预览。
- `template_preview_dark_ai_engineering_hybrid_ppt169_20260508`：生图背景 + 可编辑信息层的混合模板预览。

## 目录结构

每个示例项目通常使用以下结构：

```text
<project_name>/
├── design_spec.md       # 人类可读的设计规范
├── spec_lock.md         # 执行锁定信息
├── images/              # 图片素材
├── notes/               # 每页讲稿或备注
├── svg_output/          # Executor 原始 SVG
└── svg_final/           # 后处理后的最终 SVG
```

部分项目也会包含 `exports/`、`previews/` 或 `templates/`，用于展示最终 PPTX、接触表预览或模板验证。

## 本地预览

```bash
python -m http.server --directory examples/<project_name>/svg_final 8000
```

然后访问 `http://localhost:8000`。

也可以直接打开任意 `svg_final/*.svg`。

## 维护规则

新增示例时需要：

1. 保持标准项目结构。
2. 在 [`examples.json`](./examples.json) 的 `projects[]` 中登记项目、页面和封面。
3. 更新 `stats.examples` 与 `stats.pages`。
4. 确保 SVG 通过质量检查：

```bash
python3 skills/ppt-master/scripts/svg_quality_checker.py examples/<project_name>
```

## 相关入口

- [根 README](../README.md)
- [主工作流](../skills/ppt-master/SKILL.md)
- [模板资源](../skills/ppt-master/templates/)
- [在线预览](../viewer.html)
