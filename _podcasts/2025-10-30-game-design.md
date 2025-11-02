---
layout: single
title: "游戏设计"
---

<div style="margin-bottom: 2em;">
  <a href="/podcasts/" style="color: #007acc; text-decoration: none; font-weight: 500;">← 返回 Vivian's 播客小镇</a>
</div>


# Origin（2025-10-30）

对游戏设计的好奇，来自于25级硕士生毕业论文的指导。去年我做了一个游戏本地化主题的翻译认知过程实验，开始对游戏翻译中的各个环节进行思考。正好指导同样感兴趣的硕士学生来做毕业论文的题目。最近在讨论游戏内世界观元素的分类时，我去找了一些游戏设计的文献，发现游戏的类别、叙事方式和交互方式等都有非常大的区别，以至于业界并没有对于游戏叙事方式等有非常固定的分类。而对于译者而言，这既是一个缺失，也是一个可以深挖、研究下去的方向。因为对要翻译、本地化的文本越熟悉，我们越能摸索到解决好本地化问题的核心。

于是就有了这个对游戏设计本身进行学习的频道。我买了一些译著的纸质书，也找到了英文著作的电子版，会一并交给 NotebookLM 来进行学习。接下来，我们就开始吧。


<div class="gd-video" style="margin: 10px 0 18px;">
  <div id="gd-video-mount" style="width: 100%; aspect-ratio: 16 / 9; border: 1px solid #eee; border-radius: 10px; background: #000; display: flex; align-items: center; justify-content: center; color: #9aa7b2; font-size: 0.95rem;">正在加载视频…</div>
  <div style="font-size: 0.9rem; color: #666; margin-top: 6px;">如无法内嵌，请使用备用链接在新窗口打开：
    <a href="https://verbose-temple-e01.notion.site/Game_design-29c5a9c7a666807a94c1dfd5023e065a?source=copy_link" target="_blank" rel="noopener">在 Notion 中观看</a>
  </div>
</div>

<script>
  (function() {
    var NOTION_URL = 'https://verbose-temple-e01.notion.site/Game_design-29c5a9c7a666807a94c1dfd5023e065a?source=copy_link';
    function mountIframe() {
      var mount = document.getElementById('gd-video-mount');
      if (!mount) return;
      // 清空占位并创建 iframe
      mount.innerHTML = '';
      var iframe = document.createElement('iframe');
      iframe.src = NOTION_URL;
      iframe.setAttribute('title', 'Game Design Video');
      iframe.setAttribute('loading', 'lazy');
      iframe.style.width = '100%';
      iframe.style.height = '100%';
      iframe.style.border = '0';
      iframe.style.borderRadius = '10px';
      // 兼容没有 aspect-ratio 的浏览器
      mount.style.position = 'relative';
      if (!('aspectRatio' in document.body.style)) {
        mount.style.paddingTop = '56.25%';
        iframe.style.position = 'absolute';
        iframe.style.top = '0';
        iframe.style.left = '0';
        iframe.style.height = '100%';
      }
      mount.appendChild(iframe);
    }
    function ready(fn){
      if (document.readyState !== 'loading') { fn(); }
      else { document.addEventListener('DOMContentLoaded', fn); }
    }
    ready(function() { mountIframe(); });
  })();
</script>

## Game jargons 游戏行话

| 英文术语 | 中文术语 | 类别 |
|---------|---------|------|
| 007 Moments | 007 时刻 |  |
| 3A Game (AAA Game) | 3A 游戏 |  |
| 5W1H | 谁 (Who)、什么 (What)、何时 (When)、何地 (Where)、为何 (Why)、怎样 (How) |  |
| Ability Progression | 能力增长 |  |
| Acid Test | 决定测试 |  |
| Adrenalizer Scene | 肾上腺素注射场景 |  |
| Alignment Chart | 阵营九宫格 |  |
| Alpha, Beta, Gold | 青铜、白银、黄金 |  |
| Ammo Hunt | 寻找药械 |  |
| Amphetaminize | 刺激剂 |  |
| Aniamtic | 动态分镜 |  |
| Arcader | 街机小游戏 |  |
| Ass Cam | 臀部镜头 |  |
| Attaboys | 夸奖反馈 |  |
| Auricular Gameplay | 声音游戏 |  |
| Axonometric | 顶视 |  |
| Backcook | 意外收获 |  |
| Barneys | 呆兵乙 |  |
| Bitching Bettys | 唐僧 |  |
| Blowpast | 强推 |  |
| Blue Shoes | 蓝鞋子 |  |
| Blueprint Copying | 换皮 |  |
| Bond Sense | 邦德视感 |  |
| Botox Effect | 拉皮效应 |  |
| Branch | 游戏分支 |  |
| Branching | 多分支结构 |  |
| Breaking the Game | 破坏游戏 |  |
| Button Masher | 狂扭捣碎机 |  |
| Call-Outs | 指令 |  |
| Camedy | 假幽默 |  |
| Camera Logic | 镜头逻辑 |  |
| Car War | 小丑车 |  |
| CGI | 计算机生成图像 |  |
| Character Adventure | 角色冒险 |  |
| Cheats | 作弊码 |  |
| CIG | "听上去不错"型决策 |  |
| Cinematic | 过场动画 |  |
| Cleaning | 清洗 |  |
| Clingons | 克林贡人 |  |
| Co-Op | 合作模式 |  |
| Collectable | 收集品 |  |
| Combos | 连招 |  |
| Completion Rate | 完成度 |  |
| Conceit | 设定 |  |
| Concept Document | 概念文档 |  |
| Conditional Objective | 条件目标 |  |
| Consequences | 后果 |  |
| Critical Path | 关键路径 |  |
| Cut-Scene | 剧情画面 |  |
| Death Equivalents | "死亡情节"替代元素 |  |
| Deliverables | 交付作品 |  |
| Denting the Batmobile | 破坏蝙蝠车 |  |
| Design Document | 设计文档 |  |
| Design Wanker's Useless Concern (DWUK) | 设计师的无用想法 |  |
| Destructible Environment | 可破坏场景 |  |
| Developers | 开发商 |  |
| Diamond Branching | 钻石分支 |  |
| Directed Experience | 有引导的体验 |  |
| Dynamic Music | 动态音乐 |  |
| Elevator Pitch | 电梯推销 |  |
| Emergent Gameplay | 自发玩法 |  |
| Engine | 引擎 |  |
| Event Trigger | 事件触发 |  |
| Exposition | 展示 |  |
| Extrinsic Value | 衍生价值 |  |
| Eye Candy | 眼睛糖果 |  |
| Faux Pitch | 虚假宣传 |  |
| Fear Object | 恐惧对象 |  |
| Feature Creep | 特征蔓延 |  |
| Feedback Loop | 反馈循环 |  |
| Fetch Quest | 跑腿任务 |  |
| First-Person POV / 1st-Person | 第一人称视角 |  |
| Flow State | 心流状态 |  |
| Flushed | 冲走 |  |
| Foo | 某某 |  |
| Force | 原力 |  |
| Fractile Rewrite | 分位重写 |  |
| Freeze | 冻结 |  |
| Full-Motion Video (FMV) | 全动视频 |  |
| Fun factor | 乐趣元素 |  |
| Game Logic | 游戏逻辑 |  |
| Game Objective | 游戏目标 |  |
| Game Pride | 玩家骄傲 |  |
| Giant Rat of Sumatra | 苏门答腊巨鼠 |  |
| Gibs | 零落水下 |  |
| Glavotch | 格拉沃奇 |  |
| Gold Master | 黄金母带 |  |
| Gornished | 古董 |  |
| Granular | 颗粒 |  |
| Grognard | 老兵 |  |
| Grok | 意会 |  |
| Grounding | 接地气 |  |
| Hack and Slash | 清版 |  |
| Hat on a Hat | 叠床架屋 |  |
| Head Turn | 转头 |  |
| Hoppy-Jumpy, Platformer | 跳台子, 平台动作 |  |
| Hot Spot | 热点 |  |
| Idea Diffusion | 创意稀释 |  |
| Idea Drift | 创意漂移 |  |
| Illusion of Freedom | 自由幻觉 |  |
| Inevitable Game | 不可避免的游戏 |  |
| Instant Fun | 即刻乐趣 |  |
| Interface | 界面 |  |
| Inventory | 物品栏 |  |
| Invisible Ramp | 隐形曲线 |  |
| Isometric Camera | 等距视角 |  |
| It's a Feature! | 这是个特性! |  |
| Iterative Process | 迭代过程 |  |
| Keep It Simple, Stupid (K.I.S.S) | 保持简单，蠢货 |  |
| Keeping Alive | 别断气 |  |
| Killing Keyser | 杀掉恺撒 |  |
| Kool Idea, No Fun (K.I.N.F) | 主意很酷但不好玩的点 |  |
| Kool Idea, Not Implementable (K.I.N.I) | 主意很酷但实现不了的点子 |  |
| Laying Pipe | 铺设管子 |  |
| Learning Curve | 学习曲线 |  |
| Levels | 关卡 |  |
| Logical Idea, No Fun (L.I.N.F) | 有道理但没意思的想法 |  |
| Look and Feel | 外观和感受 |  |
| Luigi | "路易吉"卡 |  |
| Marquee | 招牌 |  |
| Mechanic | 机制 |  |
| Metastory | 元故事 |  |
| Middleware | 中间件 |  |
| Milestone | 里程碑 |  |
| Mission-Based Gameplay | 基于任务的玩法 |  |
| Monotonatic | 单调 |  |
| Mouse Fishing | "钓"鼠标 |  |
| Nonplayer Character (NPC) | 非玩家角色 |  |
| Paradigm Buster | 范式破坏者 |  |
| Parallel Design Process | 平行设计过程 |  |
| Pavlovian | 巴甫洛夫 |  |
| Payoffs | 报偿 |  |
| Pear-Shaped | 捣糊 |  |
| Pete Popcorn | 王小明 |  |
| Popcorning | 爆米花反应 |  |
| Preliminary Design Document | 初步设计文档 |  |
| Protecting an Idea | 保护创意 |  |
| Prototype | 原型 |  |
| Publishers | 游戏厂商 |  |
| Quickly Recognized Features (QRFS) | 快速理解特性 |  |
| Ragdoll | 布娃娃 |  |
| Red Shirt | 红衫 |  |
| Reference Titles | 参考作品 |  |
| Reload Learning | 重新载入学习 |  |
| Release to Manufacture (RTM) | 盘制 |  |
| Replayability (or lack thereof) | 具有重玩性 |  |
| Ripamatics | 混剪 |  |
| Rorschach | 墨迹测试 |  |
| Sandbox | 沙盒 |  |
| Schedule Monkey | 日程猴子 |  |
| Schlongbogle | 很复杂的麻烦 |  |
| Scriptment | 剧本论述 |  |
| Sense of Mystery | 掌控感 |  |
| Serendipity Factors | 巧合因素 |  |
| Snipe Hunting | 打野 |  |
| Sound Effects (SFX) | 音效 |  |
| Snags | 小点子 |  |
| Spotlight on a Turd | 给屎照光 |  |
| Standard for a Reason (SFAR) | 约定俗成的事情 |  |
| Start to Crate Ratio | 进度条时长 |  |
| Stealth Education | 隐秘教育 |  |
| Storyboard | 故事板 |  |
| Tabula Rasa or blank slate | 初始人物或空白模板 |  |
| Technical Design Document | 技术设计文档 |  |
| Tezstzlein's Law | 泰兹斯坦定律 |  |
| Third-Handed | 三只手 |  |
| Third-Person Point of View | 第三人称视角 |  |
| This Is Not My First Picnic | 这不是我的第一次野餐 |  |
| Thumb Candy | 手指糖果 |  |
| Ticking Clock | 倒计时 |  |
| Title | 作品 |  |
| Too Much Information (TMI) | 信息过量 |  |
| Toyatic | 可玩具化 |  |
| Trench Coat | 战壕大衣 |  |
| Tribivils | 系列设定 |  |
| Trunk | 主体 |  |
| Tune and Tweak | 调试修改 |  |
| Turnip Truck Gambit | 萝卜车赌博 |  |
| Turtling the Ninja | 忍者神龟化 |  |
| Unique Selling Point (USP) | 独特卖点 |  |
| Value System | 价值系统 |  |
| Vector Check | 方向检查 |  |
| Vertical Slice | 垂直切片 |  |
| Violence Equivalents | "暴力情节"替代元素 |  |
| Vision | 愿景 |  |
| Walkthrough | 攻略 |  |
| Waypoints | 路点 |  |
| Weed Eating | 铲除杂草 |  |
| Zerging | 人海战术 |  |
