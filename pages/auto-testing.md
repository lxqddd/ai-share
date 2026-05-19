---
layout: section
---

# Part 4

AI做自动化测试的一些想法

---

# 现状与痛点

<div class="grid grid-cols-2 gap-6 mt-6">

<div v-click>

### 传统自动化测试流程

<div class="mt-3 space-y-3">
<div class="p-3 rounded-lg border border-gray-500/30 bg-gray-500/5">
<div class="font-bold text-gray-400 mb-1">1. 测试同学编写用例</div>
<div class="text-sm opacity-70">Excel / 文档描述测试步骤和预期结果</div>
</div>

<div class="p-3 rounded-lg border border-gray-500/30 bg-gray-500/5">
<div class="font-bold text-gray-400 mb-1">2. 开发/测试编写自动化脚本</div>
<div class="text-sm opacity-70">将用例翻译为 Playwright / Cypress 代码，耗时长</div>
</div>

<div class="p-3 rounded-lg border border-gray-500/30 bg-gray-500/5">
<div class="font-bold text-gray-400 mb-1">3. 维护成本高</div>
<div class="text-sm opacity-70">页面变更导致脚本大面积失效，修复费时</div>
</div>
</div>

</div>

<div v-click>

### 核心痛点

<div class="mt-3 space-y-3">
<div class="p-3 rounded-lg border border-red-500/30 bg-red-500/5">
<div class="text-sm opacity-80">❌ 用例文档 → 自动化脚本的<strong>翻译成本高</strong>，需要专人维护</div>
</div>

<div class="p-3 rounded-lg border border-red-500/30 bg-red-500/5">
<div class="text-sm opacity-80">❌ UI 变更后脚本<strong>大面积失效</strong>，定位元素、时序问题排查耗时</div>
</div>

<div class="p-3 rounded-lg border border-red-500/30 bg-red-500/5">
<div class="text-sm opacity-80">❌ 测试同学<strong>不会写代码</strong>，自动化覆盖率难以提升</div>
</div>
</div>

</div>

</div>

---

# AI 驱动的自动化测试方案

<div class="mt-4 text-sm opacity-50">Claude Code + Playwright CLI · 自然语言用例直接执行</div>

<div class="grid grid-cols-2 gap-6 mt-4">

<div v-click>

### 工作流程

<div class="mt-3 space-y-3">
<div class="p-3 rounded-lg border border-green-500/30 bg-green-500/5">
<div class="font-bold text-green-400 mb-1">① 测试同学编写用例</div>
<div class="text-sm opacity-70">在文档中用自然语言描述测试步骤和预期结果，无需写代码</div>
</div>

<div class="p-3 rounded-lg border border-blue-500/30 bg-blue-500/5">
<div class="font-bold text-blue-400 mb-1">② Claude Code 直接驱动 Playwright CLI</div>
<div class="text-sm opacity-70">理解自然语言指令，直接调用 Playwright CLI 执行浏览器操作，无需生成脚本</div>
</div>

<div class="p-3 rounded-lg border border-purple-500/30 bg-purple-500/5">
<div class="font-bold text-purple-400 mb-1">③ 执行 → 分析 → 自动修复</div>
<div class="text-sm opacity-70">Claude 通过 CLI 操控浏览器，分析执行结果，失败时自动调整重试</div>
</div>
</div>

</div>

<div v-click>

### 实际操作

```bash
# 一条命令，AI 直接驱动浏览器完成测试操作
claude "使用 playwright-cli 以可见窗口模式（--headed）
       打开浏览器并打开控制台，访问
       https://elife-sit-biz.yzlcn.com/，
       登录账号 XCMT，密码 111111，
       验证码我来提供。
       登录后进入店铺下的部门和员工页面，
       编辑表格第一个员工，在昵称后追加 2 并保存。
       完成后等待指令。"
```

<div class="mt-3 p-3 rounded-lg border border-amber-500/30 bg-amber-500/5">
<div class="font-bold text-amber-400 mb-1">典型场景</div>
<ul class="text-sm opacity-70 space-y-1">
<li>新功能上线 → 测试同学补充用例 → Claude 直接驱动浏览器执行</li>
<li>UI 改版 → 用例执行失败 → Claude 自动识别变更并调整操作步骤</li>
<li>回归测试 → 每次发版前自动跑全量用例</li>
</ul>
</div>

</div>

</div>

---

# 效果对比

<div class="mt-6">

| 维度 | 传统方式 | Claude Code + Playwright |
|------|---------|------------------------|
| 用例 → 执行 | 人工编写脚本，1-2 天/批 | AI 直接驱动浏览器执行，分钟级 |
| 维护成本 | UI 变更后手动修复脚本 | AI 自动调整操作步骤，无需维护脚本 |
| 门槛 | 需要掌握 Playwright 语法 | 测试同学只需写自然语言用例 |
| 覆盖率提升 | 缓慢，受人力限制 | 快速，按需执行 |
| 失败分析 | 人工排查，耗时长 | AI 自动定位原因并重试 |

</div>

<div v-click class="mt-6 p-3 rounded-lg border border-green-500/30 bg-green-500/5 text-sm">
💡 <strong>关键价值：</strong>无需编写和维护自动化脚本，测试同学专注于<strong>用例设计和质量策略</strong>，Claude Code 直接驱动 Playwright CLI 执行测试
</div>
