# CLAUDE.md

本文件为 Claude Code (claude.ai/code) 在此仓库中工作时提供指引。

## 项目概述

基于 Slidev 的 AI 编码工具与模型技术分享演示文稿，内容为中文。

## 常用命令

```bash
pnpm run dev      # 启动开发服务器 (http://localhost:3030)
pnpm run build    # 构建静态 SPA 到 dist/
pnpm run export   # 导出为 PDF（需要 playwright-chromium）
```

包管理器：pnpm

## 架构

**主入口**：`slides.md` — 仅包含全局配置和 `src:` 引用。

**内容文件**在 `pages/` 目录下：
- `pain-points.md` — 开发者现状与痛点
- `model-comparison.md` — 国内外大模型对比（编码能力、定价）
- `tool-comparison.md` — AI 编码工具对比与团队建议

**幻灯片引入方式**：在 `slides.md` 中通过 `---\nsrc: ./pages/filename.md\n---` 引入，不要将内容内联到主文件。

## Slidev 约定

- 主题：`seriph`
- 单页 frontmatter 必须紧接 `---`，中间不能有空行，否则会被当作正文渲染
- 已使用特性：Mermaid 图表、`v-click` 动画、Tailwind 样式、`layout: section` / `layout: center`
- Slidev 语法参考：`.claude/skills/slidev/SKILL.md`

## 部署

已配置 Vercel（`vercel.json`）和 Netlify（`netlify.toml`）双平台部署，均为 SPA 模式回退到 `index.html`。
