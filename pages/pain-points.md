---
---

# 开发者的日常

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### 时间都去哪了？

<br>

```mermaid {scale: 0.75}
pie title 开发者时间分配（行业调研）
    "写业务逻辑" : 35
    "阅读/理解代码" : 20
    "写样板代码" : 15
    "查文档/搜索" : 12
    "调试/修 Bug" : 10
    "其他" : 8
```

</div>

<div class="mt-4">

<div v-click class="mb-3 p-3 rounded bg-red-500/10 border border-red-500/20">
<div class="text-red-400 font-bold text-sm mb-1">低价值重复劳动</div>
<ul class="text-xs opacity-80">
<li>CRUD、表单验证、类型定义</li>
<li>重复的组件模板和样式</li>
<li>API 对接的样板代码</li>
</ul>
</div>

<div v-click class="mb-3 p-3 rounded bg-yellow-500/10 border border-yellow-500/20">
<div class="text-yellow-400 font-bold text-sm mb-1">上下文切换成本</div>
<ul class="text-xs opacity-80">
<li>频繁在 IDE 和浏览器间切换查文档</li>
<li>Stack Overflow 来回翻找答案</li>
<li>在多个文件间跳转理解逻辑</li>
</ul>
</div>

<div v-click class="p-3 rounded bg-blue-500/10 border border-blue-500/20">
<div class="text-blue-400 font-bold text-sm mb-1">知识壁垒</div>
<ul class="text-xs opacity-80">
<li>不熟悉的框架/API 上手慢</li>
<li>遗留代码理解困难</li>
<li>跨领域开发（前端↔后端）效率低</li>
</ul>
</div>

</div>
</div>

---

# 这些场景，你是否熟悉？

<div class="mt-8 space-y-6">

<div v-click class="flex items-start gap-4 p-4 rounded-lg bg-gray-500/5">
<div class="text-3xl">🤔</div>
<div>
<div class="font-bold">"这个 API 参数是什么意思来着？"</div>
<div class="text-sm opacity-60 mt-1">打开浏览器 → 搜索 → 翻文档 → 切回 IDE → 忘了再看一遍</div>
</div>
</div>

<div v-click class="flex items-start gap-4 p-4 rounded-lg bg-gray-500/5">
<div class="text-3xl">😫</div>
<div>
<div class="font-bold">"又一个 CRUD 页面，几乎一样的逻辑"</div>
<div class="text-sm opacity-60 mt-1">复制粘贴上一个页面 → 逐个修改变量名和字段 → 手动调整差异</div>
</div>
</div>

<div v-click class="flex items-start gap-4 p-4 rounded-lg bg-gray-500/5">
<div class="text-3xl">😤</div>
<div>
<div class="font-bold">"这段遗留代码谁写的？想改但怕改出问题"</div>
<div class="text-sm opacity-60 mt-1">花大量时间理解上下文 → 小心翼翼修改 → 反复验证没有副作用</div>
</div>
</div>

<div v-click class="flex items-start gap-4 p-4 rounded-lg bg-gray-500/5">
<div class="text-3xl">😴</div>
<div>
<div class="font-bold">"测试？时间紧先不写了（技术债 +1）"</div>
<div class="text-sm opacity-60 mt-1">手动测试通过就上线 → 后续改动缺少回归保障 → Bug 率上升</div>
</div>
</div>

</div>

---
layout: center
class: text-center
---

# 如果 AI 能帮你处理这些重复劳动呢？

<div v-click class="mt-8 text-2xl font-bold bg-gradient-to-r from-blue-400 to-purple-400 bg-clip-text text-transparent">
  让开发者专注在真正需要思考的工作上
</div>

<div v-click class="mt-12 text-sm opacity-50">
  接下来，我们看看当前国内外模型的现状
</div>
