---
theme: default
background: https://images.unsplash.com/photo-1555939594-58d7cb561ad1?q=80&w=2574&auto=format&fit=crop
class: text-center
highlighter: shiki
drawings:
  persist: false
transition: slide-left
title: 小吃产品开发指南
---

# 小吃产品开发指南
### 基于JTBD的新品开发与超级单品判断模型

<div class="mt-4 text-sm opacity-80 text-gray-400">
从“消费者为什么买”到“产品应该怎么做”<br>
将消费者任务翻译为可打样、可测试、可迭代的物理属性组合
</div>

<div class="mt-12 text-xs opacity-60 text-left w-max mx-auto border-t border-gray-600 pt-4">
  <span>数据来源：</span><br>
  20260421 街访·顾客对小吃的消费需求（n=102）<br>
  20260407 街访·顾客吃炸串的场景（n=102）<br>
  20260320 店访·喜姐/青年卤味局全面定量问卷
</div>

---
layout: default
---

# 01 · 框架说明：消费者在完成什么任务？

<div class="border-l-4 border-orange-500 pl-4 py-1 bg-orange-500/10 mb-4 text-sm">
  JTBD（Jobs To Be Done）不是给产品分类，而是判断消费者在某场景下想用产品完成什么任务——同一品类可承载完全不同的消费任务。
</div>

| Job | 消费者任务核心 | 核心场景 | 典型产品 |
| :--- | :--- | :--- | :--- |
| **<span class="text-orange-500 font-bold">Job1 味觉解馋</span>** | 嘴巴想吃点有味道、有刺激、有口感的东西 | 逛街、路过、追剧、打游戏、景区、小吃街 | 鸡爪、臭豆腐、炸年糕、烤面筋 |
| **<span class="text-yellow-600 font-bold">Job2 肉感解馋</span>** | 想吃点肉，吃得更爽、更有满足感 | 下班后、社区回家途中、朋友小聚、独处 | 大鸡排、鸡腿、大肉串、小酥肉 |
| **<span class="text-green-600 font-bold">Job3 解决一餐</span>** | 这一顿要吃饱、吃好、效率高 | 工作餐、加班餐、通勤餐、单人快餐 | 鸡排饭、炸串粉面、螺蛳粉套餐 |
| **<span class="text-blue-500 font-bold">Job4 完善餐桌</span>** | 家里/桌上这一顿还缺东西，补充餐桌组件 | 社区、回家路上、家庭晚餐、早餐补充 | 卤牛肉、棒棒鸡、包子、熟食拼盘 |

<div class="grid grid-cols-2 gap-4 mt-6">
  <div class="bg-gray-100 dark:bg-gray-800 p-4 rounded text-sm">
    <div class="text-orange-500 font-bold mb-2">核心结论</div>
    <span class="text-orange-500">Job1</span> & <span class="text-yellow-600">Job2</span> 更接近<strong>即时欲望</strong>，最依赖现场触发。<br>
    <span class="text-green-600">Job3</span> & <span class="text-blue-500">Job4</span> 更接近<strong>餐食解决</strong>，有前置计划。
  </div>
  <div class="bg-gray-100 dark:bg-gray-800 p-4 rounded text-sm">
    <div class="text-orange-500 font-bold mb-2">研发核心问题</div>
    它是帮消费者解馋、吃肉、吃饭，还是补全餐桌？<br>
    <span class="opacity-70 text-xs">不能只问“产品好不好吃”，而要先确定它服务的Job。</span>
  </div>
</div>

---
layout: default
---

# 02 · 边界定义：JTBD的消费者心智与场景边界

| 维度 | <span class="text-orange-500">Job1 味觉解馋</span> | <span class="text-yellow-600">Job2 肉感解馋</span> | <span class="text-green-600">Job3 解决一餐</span> | <span class="text-blue-500">Job4 完善餐桌</span> |
| :--- | :--- | :--- | :--- | :--- |
| **消费者心智** | "嘴巴想吃点什么" | "想吃点肉，吃爽一点" | "我这一顿吃什么" | "家里/桌上这一顿还缺点什么" |
| **主要触发** | 看见、闻到、路过 | 想奖励自己、下班放松 | 到饭点、饿了、工作餐 | 回家路上、准备晚餐 |
| **产品角色** | 随机解馋小吃 | 有肉感的满足型小吃 | 可独立承担一顿饭 | 家庭/餐桌的一部分 |
| **是否必须饱** | <span class="opacity-50">不需要</span> | <span class="opacity-50">不一定</span> | **必须能顶一顿** | 不一定，补全餐桌即可 |
| **消费单位** | 个人即时消费 | 个人或小范围分享 | 个人一餐为主 | 家庭/多人/餐桌为主 |
| **决策特征** | **最随机，依赖现场** | 半随机，有一定欲望 | **明确前置决策** | 前置性强，计划性 |
| **典型价格带**| 3—15元 | 15—40元 | 20—45元/餐 | 15—50元/盒 |

---
layout: default
---

# 03 · 产品属性（上）：用物理属性指导研发

情绪价值用于理解消费者，物理属性用于指导研发打样。

| 产品属性 | 含义 | 正面例子 | 反向例子 |
| :--- | :--- | :--- | :--- |
| **味型刺激度** | 麻/辣/酸/臭/甜辣/卤香等味型强度 | 臭豆腐、藤椒鸡爪、甜辣炸年糕 | 清淡白煮肉、无味素菜 |
| **口感层次** | 脆/糯/弹/韧/酥/嫩/嚼劲等变化 | 炸年糕外脆内糯、鸡爪带筋 | 单一软烂、口感塌陷 |
| **视觉/嗅觉诱惑力** | 色泽、油光、明档、炸烤卤香 | 明档炸串、热卤柜、烤串烟火气 | 冷冰冰、颜色暗、无香味 |
| **小份轻负担** | 适合小份购买随手吃、不怕浪费 | 小串、鸡爪单份、炸豆皮小份 | 大份套餐、整只大菜 |
| **肉块感/蛋白** | 是否有大块、厚切、明显蛋白质 | 大鸡排、大鸡腿、大肉串、卤牛肉 | 肉末感、碎肉感、看不到肉 |
| **油脂/焦香强度** | 炸、烤、煎、美拉德、脆皮 | 炸鸡腿、烤肉串、小酥肉 | 水煮、低脂、无焦香 |
| **一餐份量感** | 体积、重量、热量是否足以顶一顿 | 鸡排饭、螺蛳粉、大份炸串粉面 | 两三串小吃、一小盒零嘴 |

---
layout: default
---

# 03 · 产品属性（下）：用物理属性指导研发

| 产品属性 | 含义 | 正面例子 | 反向例子 |
| :--- | :--- | :--- | :--- |
| **膳食完整度** | 具备主食+蛋白+蔬菜+汤饮 | 鸡排饭+小菜+汤，粉面+青菜 | 只有炸物/肉，无主食无配菜 |
| **价格/份量价值感** | 份量、肉量让人觉得值 | 大份鸡排套餐、加量炸串 | 价格高但量少、组合单薄 |
| **主食适配度** | 适合配碳水，提升主食体验 | 卤牛肉、棒棒鸡、小酥肉 | 甜品、炸年糕、烤面筋 |
| **成菜感/可上桌性** | 像完整菜品，适合成盘成盒 | 卤味拼盘、棒棒鸡、包子 | 单根串、边走边吃小吃 |
| **口味普适性** | 不过辣/麻/臭/怪，多人可接受 | 酱香卤味、藤椒微辣、原味 | 极辣、重臭、重麻、强猎奇 |
| **复热适配性** | 外带不软/腥/柴，复热好吃 | 卤牛肉、卤味拼盘、冷吃鸡 | 炸物回软、粉面坨掉外溢 |
| **食用便利性** | 少骨少汁不脏手，方便分食 | 鸡柳、切块鸡排、卤牛肉片 | 鸭头、鸡爪、带刺带壳产品 |

<div class="mt-4 p-3 bg-blue-500/10 border border-blue-500/20 rounded text-sm">
  <strong>使用说明：</strong>这14个属性是新品评分的基础变量。每个属性在打样时都要有对应的物理体现——不是说"这个产品解馋"，而是说"味型刺激度是4，口感层次是3，视觉诱惑力是5"。
</div>

---
layout: default
---

# 04 · 权重矩阵：产品属性 × 四类JTBD适配权重

评分含义：`2` 门槛属性；`1` 关键增强；`0` 不重要；`-1` 过强会干扰；`-2` 不兼容。

<div class="text-xs grid grid-cols-2 gap-4 mt-4">
<div>

| 产品属性 | <span class="text-orange-500">J1</span> | <span class="text-yellow-600">J2</span> | <span class="text-green-600">J3</span> | <span class="text-blue-500">J4</span> |
| :--- | :---: | :---: | :---: | :---: |
| **味型刺激度** | 2 | 1 | -1 | 0 |
| **口感层次** | 2 | 1 | 1 | 1 |
| **视觉/嗅觉诱惑力**| 2 | 1 | 1 | 1 |
| **小份轻负担** | 2 | -1 | -1 | 0 |
| **肉块感/蛋白** | 0 | 2 | 1 | 1 |
| **油脂/酥脆强度** | 1 | 2 | 0 | -1 |
| **一餐份量感** | -1 | 0 | 2 | 0 |

</div>
<div>

| 产品属性 | <span class="text-orange-500">J1</span> | <span class="text-yellow-600">J2</span> | <span class="text-green-600">J3</span> | <span class="text-blue-500">J4</span> |
| :--- | :---: | :---: | :---: | :---: |
| **膳食完整度** | -1 | 0 | 2 | 1 |
| **价格价值感** | 0 | 2 | 2 | 1 |
| **主食适配度** | -1 | 0 | 1 | 2 |
| **成菜感/上桌性** | 0 | 0 | 1 | 2 |
| **口味普适性** | -1 | 0 | 1 | 2 |
| **复热适配性** | 0 | 0 | 1 | 2 |
| **食用便利性** | 1 | 0 | 2 | 1 |

</div>
</div>

---
layout: default
---

# 05 · 评价方法：跨Job潜力判断标准

计算公式：**新品Job得分 = Σ（属性强度 1-5分 × 该属性适配权重）**

<div class="grid grid-cols-2 gap-6 mt-6">
  <div>
    <h3 class="text-lg font-bold mb-2">跨Job潜力判断</h3>
    <ul class="list-disc pl-4 text-sm leading-loose">
      <li><span class="text-green-500 font-bold">次高/最高 ≥70%，且最高绝对分≥25</span>：具备跨Job潜力，可作超级单品方向。</li>
      <li><span class="text-orange-500 font-bold">次高/最高 &lt;70%，或最高绝对分&lt;25</span>：跨Job信号弱，优先聚焦主力Job做深。</li>
      <li><span class="text-red-500 font-bold">四个Job均低于15分</span>：产品没有清晰任务，需重新定位或重打样。</li>
    </ul>
  </div>
  <div class="bg-gray-100 dark:bg-gray-800 p-4 rounded text-sm">
    <h3 class="text-orange-500 font-bold mb-2">示例：大鸡排（明档现炸）</h3>
    <ul class="space-y-2">
      <li>🥇 <span class="font-bold text-yellow-600">Job2 肉感解馋 (39分)</span></li>
      <li>🥈 Job3 解决一餐 (36分) - <span class="opacity-70">比例92%，跨Job潜力强，适合加主食转套餐</span></li>
      <li>🥉 Job4 完善餐桌 (33分)</li>
      <li>4️⃣ Job1 味觉解馋 (27分) - <span class="opacity-70">非小份、普适性高，不具备爆点引流优势</span></li>
    </ul>
  </div>
</div>

---
layout: default
---

# 06 · 超级单品：六类跨Job产品形成路径

<div class="grid grid-cols-2 gap-4 text-sm mt-4">
  <div class="border border-gray-200 dark:border-gray-700 p-3 rounded">
    <div class="font-bold mb-1"><span class="text-orange-500">Job1</span> + <span class="text-yellow-600">Job2</span> 解馋爆品型</div>
    <div class="italic opacity-70 mb-2">看见想买，吃起来过瘾</div>
    代表：大鸡排、大肉串、烤鸡架<br>角色：门店招牌、提升客单
  </div>
  <div class="border border-gray-200 dark:border-gray-700 p-3 rounded">
    <div class="font-bold mb-1"><span class="text-yellow-600">Job2</span> + <span class="text-green-600">Job3</span> 肉感正餐型</div>
    <div class="italic opacity-70 mb-2">有肉感，也能顶一顿</div>
    代表：鸡排饭、炸串粉面<br>角色：工作餐、高频复购
  </div>
  <div class="border border-gray-200 dark:border-gray-700 p-3 rounded">
    <div class="font-bold mb-1"><span class="text-yellow-600">Job2</span> + <span class="text-blue-500">Job4</span> 肉感补餐型</div>
    <div class="italic opacity-70 mb-2">有肉感，买回家能上桌</div>
    代表：卤牛肉切片、酱鸭腿<br>角色：卤味店主力、家庭蛋白
  </div>
  <div class="border border-gray-200 dark:border-gray-700 p-3 rounded">
    <div class="font-bold mb-1"><span class="text-green-600">Job3</span> + <span class="text-blue-500">Job4</span> 正餐双场景型</div>
    <div class="italic opacity-70 mb-2">单人能吃一顿，家庭能上一桌</div>
    代表：棒棒鸡（饭/盒装）、鸡排（套餐/盒）<br>角色：品牌主力，一品两卖
  </div>
  <div class="border border-gray-200 dark:border-gray-700 p-3 rounded">
    <div class="font-bold mb-1"><span class="text-orange-500">Job1</span> + <span class="text-blue-500">Job4</span> 社区顺手补餐</div>
    <div class="italic opacity-70 mb-2">看见想买，带回家补全餐桌</div>
    代表：小米凉糕、炸物小拼盘
  </div>
  <div class="border border-red-500/30 p-3 rounded bg-red-500/5">
    <div class="font-bold mb-1 text-red-500">Job1 + Job3 触发型正餐 (难度最高)</div>
    <div class="italic opacity-70 mb-2">被诱惑触发，进店解决一顿饭</div>
    代表：炸串引流 + 粉面套餐成单。<strong>通常需要两步连带，而非单一产品。</strong>
  </div>
</div>

---
layout: center
---

# 07 · 交互测评工具：多品类模型演算

请选择下方预设产品，或直接拖动滑块，实时计算 14 项物理属性组合下的 JTBD 得分。

<script setup>
import { reactive, computed, ref } from 'vue'

const presets = {
  'custom': [3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3],
  'xijie': [4, 4, 4, 5, 1, 3, 1, 1, 3, 1, 1, 4, 1, 4], // 喜姐炸年糕
  'linyu': [3, 4, 5, 2, 5, 5, 2, 1, 5, 2, 1, 5, 2, 3], // 临渝炸鸡腿
  'jiliu': [4, 4, 4, 4, 3, 4, 2, 1, 4, 1, 1, 4, 1, 5], // 鸡柳大人三合一
  'zhengxin': [3, 3, 5, 1, 5, 5, 3, 1, 5, 1, 1, 4, 1, 4], // 正新鸡排
  'juewei': [5, 4, 3, 3, 2, 2, 1, 1, 2, 2, 3, 3, 5, 1], // 绝味鸭脖
  'ziyan': [3, 3, 4, 1, 5, 2, 3, 2, 4, 5, 5, 4, 5, 4], // 紫燕百味鸡
  'luosifen': [5, 5, 5, 1, 2, 4, 5, 4, 4, 5, 3, 2, 1, 2] // 螺蛳粉
}

const currentPreset = ref('custom')

const attrs = reactive([
  { name: '味型刺激度', val: 3 }, { name: '口感层次', val: 3 },
  { name: '视觉/嗅觉诱惑力', val: 3 }, { name: '小份轻负担', val: 3 },
  { name: '肉块感/蛋白存在感', val: 3 }, { name: '油脂/酥脆强度', val: 3 },
  { name: '一餐份量感', val: 3 }, { name: '膳食完整度', val: 3 },
  { name: '价格/份量价值感', val: 3 }, { name: '主食适配度', val: 3 },
  { name: '成菜感/可上桌性', val: 3 }, { name: '口味普适性', val: 3 },
  { name: '温度/复热适配性', val: 3 }, { name: '食用便利性', val: 3 }
])

const loadPreset = () => {
  const vals = presets[currentPreset.value]
  attrs.forEach((a, i) => a.val = vals[i])
}

const w1 = [2, 2, 2, 2, 0, 1, -1, -1, 0, -1, 0, -1, 0, 1]
const w2 = [1, 1, 1, -1, 2, 2, 0, 0, 2, 0, 0, 0, 0, 0]
const w3 = [-1, 1, 1, -1, 1, 0, 2, 2, 2, 1, 1, 1, 1, 2]
const w4 = [0, 1, 1, 0, 1, -1, 0, 1, 1, 2, 2, 2, 2, 1]

const scores = computed(() => {
  let s = [0, 0, 0, 0]
  attrs.forEach((a, i) => {
    s[0] += a.val * w1[i]
    s[1] += a.val * w2[i]
    s[2] += a.val * w3[i]
    s[3] += a.val * w4[i]
  })
  return s
})

const conclusion = computed(() => {
  const s = scores.value;
  const sorted = s.map((val, i) => ({val, i})).sort((a,b) => b.val - a.val);
  const top = sorted[0];
  const second = sorted[1];
  const jobNames = ['Job1 味觉解馋', 'Job2 肉感解馋', 'Job3 解决一餐', 'Job4 完善餐桌'];
  
  if (s.every(v => v < 15)) return "⚠ 产品得分均低于15分，缺乏清晰应用场景，建议重新定位打样。";
  
  let ratio = top.val > 0 ? (second.val / top.val * 100).toFixed(0) : 0;
  let cross = ratio >= 70 && top.val >= 25;
  
  let text = `🎯 主力场景判定为 **${jobNames[top.i]}**（${top.val}分）。<br>`;
  if (cross) {
    text += `🚀 具备跨场景潜力：次高场景为 **${jobNames[second.i]}**（${second.val}分，比值 ${ratio}%），可作为复合型超级单品。`;
  } else {
    text += `🔒 跨场景信号偏弱（比值 ${ratio}%），建议优先打透主力 Job，避免定位发散。`;
  }
  return text;
})
</script>

<div class="my-4 flex items-center justify-center gap-4 bg-gray-50 dark:bg-gray-800 py-2 rounded">
  <span class="text-sm font-bold opacity-80">加载对标品类模型：</span>
  <select v-model="currentPreset" @change="loadPreset" class="px-3 py-1 border rounded text-sm text-black">
    <option value="custom">-- 自定义测算 --</option>
    <option value="xijie">喜姐炸年糕 (强引流/弱复热)</option>
    <option value="linyu">临渝炸鸡腿 (强肉感/高性价比)</option>
    <option value="jiliu">鸡柳大人三合一 (高便利/随手买)</option>
    <option value="zhengxin">正新鸡排 (高肉感/强饱腹)</option>
    <option value="juewei">绝味鸭脖 (极强刺激/低便利)</option>
    <option value="ziyan">紫燕百味鸡 (强主食适配/餐桌王者)</option>
    <option value="luosifen">螺蛳粉 (极强饱腹/低普适)</option>
  </select>
</div>

<div class="grid grid-cols-2 gap-x-8 gap-y-1 text-xs">
  <div v-for="(item, index) in attrs" :key="index" class="flex justify-between items-center border-b border-gray-200 dark:border-gray-700 pb-1">
    <label class="w-32">{{ item.name }}</label>
    <input type="range" v-model.number="item.val" min="1" max="5" class="w-24 accent-orange-500 cursor-pointer">
    <span class="w-4 text-right font-bold text-orange-500">{{ item.val }}</span>
  </div>
</div>

<div class="grid grid-cols-4 gap-4 mt-4 text-center">
  <div class="p-2 rounded transition-all" :class="Math.max(...scores) === scores[0] ? 'bg-orange-500 text-white font-bold scale-105' : 'bg-gray-100 dark:bg-gray-800'">
    <div class="text-xs">Job1 (味觉)</div><div class="text-xl">{{ scores[0] }}</div>
  </div>
  <div class="p-2 rounded transition-all" :class="Math.max(...scores) === scores[1] ? 'bg-yellow-600 text-white font-bold scale-105' : 'bg-gray-100 dark:bg-gray-800'">
    <div class="text-xs">Job2 (肉感)</div><div class="text-xl">{{ scores[1] }}</div>
  </div>
  <div class="p-2 rounded transition-all" :class="Math.max(...scores) === scores[2] ? 'bg-green-600 text-white font-bold scale-105' : 'bg-gray-100 dark:bg-gray-800'">
    <div class="text-xs">Job3 (一餐)</div><div class="text-xl">{{ scores[2] }}</div>
  </div>
  <div class="p-2 rounded transition-all" :class="Math.max(...scores) === scores[3] ? 'bg-blue-500 text-white font-bold scale-105' : 'bg-gray-100 dark:bg-gray-800'">
    <div class="text-xs">Job4 (餐桌)</div><div class="text-xl">{{ scores[3] }}</div>
  </div>
</div>

<div class="mt-4 p-3 bg-gray-50 dark:bg-gray-900 border border-gray-200 dark:border-gray-700 rounded text-sm text-left" v-html="conclusion"></div>