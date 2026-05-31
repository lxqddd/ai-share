---
layout: section
---

# Part 2

AI 编码工具对比

---

# AI 编码工具分类

<div class="grid grid-cols-2 gap-4 mt-6">

<div v-click class="p-4 rounded-lg border border-blue-500/30 bg-blue-500/5">
<div class="flex items-center gap-2 mb-3">
<span class="text-lg">🖥️</span>
<span class="font-bold text-blue-400">IDE 内嵌</span>
</div>
<div class="text-sm space-y-1">
<div><span class="opacity-50">代表：</span>Cursor / GitHub Copilot / Windsurf</div>
<div><span class="opacity-50">特点：</span>嵌入编辑器，行内补全 + 对话 + Agent 模式</div>
<div><span class="opacity-50">适合：</span>日常编码辅助，上手门槛最低</div>
</div>
</div>

<div v-click class="p-4 rounded-lg border border-orange-500/30 bg-orange-500/5">
<div class="flex items-center gap-2 mb-3">
<span class="text-lg">⌨️</span>
<span class="font-bold text-orange-400">CLI Agent</span>
</div>
<div class="text-sm space-y-1">
<div><span class="opacity-50">代表：</span>Claude Code / OpenCode / Codex CLI</div>
<div><span class="opacity-50">特点：</span>终端运行，自主读写文件、执行命令、自动调试</div>
<div><span class="opacity-50">适合：</span>复杂多步骤任务、重构、项目级操作</div>
</div>
</div>

<div v-click class="p-4 rounded-lg border border-green-500/30 bg-green-500/5">
<div class="flex items-center gap-2 mb-3">
<span class="text-lg">🔍</span>
<span class="font-bold text-green-400">代码审查</span>
</div>
<div class="text-sm space-y-1">
<div><span class="opacity-50">代表：</span>CodeRabbit / Claude Code Review</div>
<div><span class="opacity-50">特点：</span>自动 PR Review，安全漏洞检测，代码质量评估</div>
<div><span class="opacity-50">适合：</span>团队协作，保障代码质量</div>
</div>
</div>

<div v-click class="p-4 rounded-lg border border-purple-500/30 bg-purple-500/5">
<div class="flex items-center gap-2 mb-3">
<span class="text-lg">🎨</span>
<span class="font-bold text-purple-400">低代码/生成</span>
</div>
<div class="text-sm space-y-1">
<div><span class="opacity-50">代表：</span>v0 by Vercel</div>
<div><span class="opacity-50">特点：</span>自然语言描述 → 完整前端应用，可视化 + 代码生成</div>
<div><span class="opacity-50">适合：</span>快速原型、前端页面、MVP 搭建</div>
</div>
</div>

</div>

<div v-click class="mt-4 p-2 rounded bg-gray-500/5 text-sm opacity-70">
<strong>核心趋势：</strong>工具从"代码补全"进化到"自主 Agent" — 不只是建议代码，而是能理解需求、读写文件、执行命令、自动调试
</div>

---

# IDE 内嵌工具：Cursor vs Copilot vs Windsurf

<div class="grid grid-cols-3 gap-4 mt-6">

<div v-click class="p-4 rounded-lg border border-blue-500/30 bg-blue-500/5">
<div class="flex items-center gap-2 mb-3">
<span class="text-xl">🔵</span>
<span class="font-bold">Cursor</span>
</div>
<div class="text-sm space-y-1">
<div><span class="opacity-50">模式：</span>Tab 补全 + Agent 模式</div>
<div><span class="opacity-50">模型：</span>Claude / GPT / 自选</div>
<div><span class="opacity-50">亮点：</span>多文件编辑、自动执行终端命令、错误自修复</div>
<div class="mt-2 text-xs opacity-50">价格：$20/月 Pro</div>
</div>
</div>

<div v-click class="p-4 rounded-lg border border-green-500/30 bg-green-500/5">
<div class="flex items-center gap-2 mb-3">
<span class="text-xl">🟢</span>
<span class="font-bold">GitHub Copilot</span>
</div>
<div class="text-sm space-y-1">
<div><span class="opacity-50">模式：</span>行内补全 + Chat</div>
<div><span class="opacity-50">模型：</span>GPT-4o / o3 / Claude</div>
<div><span class="opacity-50">亮点：</span>VS Code/JetBrains 原生集成，生态最广，免费版可用</div>
<div class="mt-2 text-xs opacity-50">价格：免费 / $10/月 / $19/月</div>
</div>
</div>

<div v-click class="p-4 rounded-lg border border-purple-500/30 bg-purple-500/5">
<div class="flex items-center gap-2 mb-3">
<span class="text-xl">🟣</span>
<span class="font-bold">Windsurf</span>
</div>
<div class="text-sm space-y-1">
<div><span class="opacity-50">模式：</span>Cascade 自动流</div>
<div><span class="opacity-50">模型：</span>Claude / GPT / 自选</div>
<div><span class="opacity-50">亮点：</span>多文件自动编辑 + 终端执行，价格有优势</div>
<div class="mt-2 text-xs opacity-50">价格：免费 / $15/月 Pro</div>
</div>
</div>

</div>

<div v-click class="mt-4 p-3 rounded bg-blue-500/10 border border-blue-500/20 text-sm">
💡 <strong>选型参考：</strong>日常编码补全 → <strong>Copilot</strong>（轻量免费）；深度重构 + Agent 任务 → <strong>Cursor</strong>（最成熟）；性价比 → <strong>Windsurf</strong>
</div>

---

# CLI Agent 工具：Claude Code vs OpenCode

<div class="grid grid-cols-2 gap-6 mt-4" style="grid-template-rows: 1fr auto;">

<div v-click style="grid-row: 1;">

<div class="p-4 rounded-lg border border-orange-500/30 bg-orange-500/5 h-full">
<div class="flex items-center gap-2 mb-3">
<span class="text-xl">🟠</span>
<span class="text-lg font-bold text-orange-400">Claude Code</span>
<span class="text-xs opacity-50">Anthropic</span>
</div>
<div class="text-sm space-y-1.5">
<div><span class="opacity-50">定位：</span>终端里的 AI 结对编程，理解整个项目上下文</div>
<div><span class="opacity-50">能力：</span>自主读写文件、执行命令、Git 操作、Code Review</div>
<div><span class="opacity-50">模型：</span>原生 Claude 系列，可通过 CC Switch 接入第三方模型</div>
<div><span class="opacity-50">价格：</span>按 Token 计费（Opus $5/$25）或 Max 订阅 $100~200/月</div>
</div>
</div>

</div>

<div v-click style="grid-row: 1;">

<div class="p-4 rounded-lg border border-teal-500/30 bg-teal-500/5 h-full">
<div class="flex items-center gap-2 mb-3">
<span class="text-xl">🟢</span>
<span class="text-lg font-bold text-teal-400">OpenCode</span>
<span class="text-xs opacity-50">开源</span>
</div>
<div class="text-sm space-y-1.5">
<div><span class="opacity-50">定位：</span>开源 AI 编程 Agent，Go 编写，TUI 界面</div>
<div><span class="opacity-50">能力：</span>多文件编辑、LSP 深度集成、兼容 Tmux/SSH 远程</div>
<div><span class="opacity-50">模型：</span>自由切换 Claude / GPT / DeepSeek 等任意模型</div>
<div><span class="opacity-50">价格：</span>开源免费，按各模型 API 计费</div>
</div>
</div>

</div>

<div v-click style="grid-column: 1; grid-row: 2;">

```bash
claude "添加用户登录页面"
claude "运行测试并修复失败用例"
claude "review 这个 PR"
```

</div>

<div v-click style="grid-column: 2; grid-row: 2;">

```bash
opencode "重构错误处理模块"
opencode "编写单元测试"
opencode "分析项目架构"
```

</div>

</div>

<div v-click class="mt-4 p-3 rounded bg-yellow-500/10 border border-yellow-500/20 text-sm">
💡 <strong>选型建议：</strong>追求编码能力 → <strong>Claude Code</strong>（最强）；搭配国产模型 / 开源方案 → <strong>OpenCode</strong>（免费 + 模型可选）
</div>

