---
layout: section
---

# Part 4

AI做自动化测试的一些想法

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

# 总结与展望

<div class="grid grid-cols-2 gap-6 mt-6">

<div>

### 本次分享回顾

<div class="mt-3 space-y-3">
<div class="p-3 rounded-lg border border-blue-500/30 bg-blue-500/5">
<div class="font-bold text-blue-400 mb-1">Part 1 - 现状与痛点</div>
<div class="text-sm opacity-70">开发者日常面临的编码效率瓶颈</div>
</div>

<div class="p-3 rounded-lg border border-blue-500/30 bg-blue-500/5">
<div class="font-bold text-blue-400 mb-1">Part 2 - 大模型对比</div>
<div class="text-sm opacity-70">国内外主流模型编码能力与性价比分析</div>
</div>

<div class="p-3 rounded-lg border border-blue-500/30 bg-blue-500/5">
<div class="font-bold text-blue-400 mb-1">Part 3 - 工具与实战</div>
<div class="text-sm opacity-70">AI 编码工具选型与 Claude Code 使用技巧</div>
</div>

<div class="p-3 rounded-lg border border-blue-500/30 bg-blue-500/5">
<div class="font-bold text-blue-400 mb-1">Part 4 - 自动化测试</div>
<div class="text-sm opacity-70">AI 驱动的无脚本自动化测试方案</div>
</div>
</div>

</div>

<div v-click>

### 行动建议

<div class="mt-3 space-y-3">
<div class="p-3 rounded-lg border border-green-500/30 bg-green-500/5">
<div class="text-sm opacity-80">✅ 试用 Claude Code，体验 AI 辅助编码的效率提升</div>
</div>

<div class="p-3 rounded-lg border border-green-500/30 bg-green-500/5">
<div class="text-sm opacity-80">✅ 从简单场景起步，逐步将 AI 融入日常开发流程</div>
</div>

<div class="p-3 rounded-lg border border-green-500/30 bg-green-500/5">
<div class="text-sm opacity-80">✅ 测试团队可先行探索 AI + Playwright 的自动化测试方案</div>
</div>

<div class="p-3 rounded-lg border border-green-500/30 bg-green-500/5">
<div class="text-sm opacity-80">✅ 团队内部分享实践经验，共同优化 AI 工具使用方式</div>
</div>
</div>

</div>

</div>

---
layout: center
class: text-center
---

# 感谢聆听

<div class="opacity-50 mt-4 text-sm">欢迎交流与讨论</div>
