---
title: "2026-07-28 本地化商业模拟 · AI赋能教育游戏设计"
collection: talks
type: "Talk"
permalink: /talks/2026-07-28
venue: "人工智能赋能教育学术交流会 / 教育游戏设计工作坊"
date: 2026-07-28
location: "Beijing"
author_profile: false
classes: wide
excerpt: "以【本地化商业模拟】游戏为例，汇报一门AI赋能教育游戏的课程定位、决策机制与 AI 应用。"
---


<style>
@import url('https://fonts.googleapis.com/css2?family=Outfit:wght@500;700;800&family=Noto+Sans+SC:wght@400;500;700&display=swap');

/* 演示页：突破主题窄栏，贴近 16:9 宽屏 */
.masthead {
  padding-top: 0.35rem !important;
  padding-bottom: 0.35rem !important;
}
#main {
  max-width: min(1440px, 98vw) !important;
  margin-top: 0.4rem !important;
  padding-left: 0.75rem !important;
  padding-right: 0.75rem !important;
}
.page {
  float: none !important;
  width: 100% !important;
  max-width: none !important;
  padding: 0 !important;
  margin: 0 !important;
}
.page__inner-wrap > header,
.page__meta,
.page__footer {
  display: none !important;
}
.page__content {
  padding-bottom: 0 !important;
}

.deck-note {
  font-size: 0.85rem; color: #64748b; margin: 0 0 1.25rem;
}
.deck-note kbd {
  background: #e2e8f0; border-radius: 4px; padding: 0.1rem 0.4rem;
  font-size: 0.8rem; font-family: ui-monospace, monospace;
}

.deck {
  --ink: #0f2744;
  --ink-soft: #334155;
  --blue: #1e5a96;
  --blue-bright: #2c6bac;
  --sky: #e8f1fa;
  --teal: #0f6e56;
  --teal-soft: #d8f3ea;
  --amber: #9a6700;
  --amber-soft: #fff3d6;
  --coral: #b42318;
  --coral-soft: #fce8e6;
  --fog: #f1f5f9;
  --line: #d0dbe8;
  --white: #ffffff;
  font-family: "Noto Sans SC", "PingFang SC", "Microsoft YaHei", sans-serif;
  color: var(--ink-soft);
  line-height: 1.4;
  width: 100%;
  max-width: min(1360px, 100%);
  margin: 0 auto 1.5rem;
}

.deck .slide {
  scroll-margin-top: 0.6rem;
  background: var(--white);
  border: 1px solid var(--line);
  border-radius: 14px;
  overflow: hidden;
  margin-bottom: 0.85rem;
  box-shadow: 0 6px 22px rgba(15, 39, 68, 0.05);
}

.deck .slide-bar {
  height: 5px;
  background: linear-gradient(90deg, var(--blue) 0%, #4a90c8 55%, #7eb8d8 100%);
}
.deck .slide-bar.teal { background: linear-gradient(90deg, #0f6e56, #3d9b7a); }
.deck .slide-bar.amber { background: linear-gradient(90deg, #9a6700, #d4a017); }
.deck .slide-bar.coral { background: linear-gradient(90deg, #b42318, #e05a4f); }
.deck .slide-bar.ink { background: linear-gradient(90deg, #0f2744, #2c6bac); }

.deck .slide-body { padding: 1rem 1.65rem 1.1rem; }

.deck .slide-num {
  display: inline-flex; align-items: center; gap: 0.4rem;
  font-family: Outfit, sans-serif;
  font-size: 0.68rem; font-weight: 700; letter-spacing: 0.08em;
  text-transform: uppercase; color: var(--blue-bright);
  margin-bottom: 0.3rem;
}
.deck .slide-num span {
  background: var(--sky); color: var(--blue);
  border-radius: 999px; padding: 0.1rem 0.5rem;
}

.deck h2.slide-title {
  font-family: Outfit, "Noto Sans SC", sans-serif;
  font-size: 1.35rem; font-weight: 800; color: var(--ink);
  margin: 0 0 0.55rem; line-height: 1.2; border: none; padding: 0;
}
.deck h3 {
  font-family: Outfit, "Noto Sans SC", sans-serif;
  font-size: 0.95rem; font-weight: 700; color: var(--ink);
  margin: 0.65rem 0 0.35rem; border: none; padding: 0;
}
.deck p { margin: 0 0 0.45rem; font-size: 0.9rem; }
.deck strong { color: var(--ink); font-weight: 700; }

/* Hero */
.deck .hero {
  background:
    radial-gradient(ellipse 80% 60% at 100% 0%, rgba(44,107,172,0.18), transparent 55%),
    radial-gradient(ellipse 50% 40% at 0% 100%, rgba(15,110,86,0.12), transparent 50%),
    linear-gradient(160deg, #0f2744 0%, #1a3f6b 48%, #1e5a96 100%);
  color: #e8eef6;
  border: none;
}
.deck .hero .slide-body {
  padding: 1.5rem 2rem 1.4rem;
  display: grid;
  grid-template-columns: 1.4fr 1fr;
  gap: 1rem 2rem;
  align-items: center;
}
.deck .hero .eyebrow {
  font-family: Outfit, sans-serif;
  font-size: 0.72rem; font-weight: 700; letter-spacing: 0.12em;
  text-transform: uppercase; color: #9ec0e0; margin-bottom: 0.45rem;
  grid-column: 1 / -1;
}
.deck .hero h1 {
  font-family: Outfit, "Noto Sans SC", sans-serif;
  font-size: clamp(1.55rem, 2.6vw, 2.15rem);
  font-weight: 800; color: #fff; margin: 0 0 0.45rem;
  line-height: 1.15; border: none;
}
.deck .hero .lede {
  font-size: 0.95rem; color: #c5d6e8; max-width: none; margin-bottom: 0;
}
.deck .hero-meta {
  display: flex; flex-wrap: wrap; gap: 0.4rem;
  align-content: center;
}
.deck .chip {
  display: inline-block;
  background: rgba(255,255,255,0.12);
  border: 1px solid rgba(255,255,255,0.22);
  border-radius: 8px;
  padding: 0.3rem 0.65rem;
  font-size: 0.78rem; color: #e8eef6;
}
.deck .chip.solid {
  background: #fff; color: var(--blue); font-weight: 700; border-color: #fff;
}

/* Cards / grids */
.deck .grid-2 {
  display: grid; grid-template-columns: 1fr 1fr; gap: 0.6rem;
}
.deck .grid-3 {
  display: grid; grid-template-columns: repeat(3, 1fr); gap: 0.55rem;
}
.deck .grid-4 {
  display: grid; grid-template-columns: repeat(4, 1fr); gap: 0.5rem;
}
@media (max-width: 800px) {
  .deck .grid-2, .deck .grid-3, .deck .grid-4 { grid-template-columns: 1fr; }
  .deck .hero .slide-body { grid-template-columns: 1fr; padding: 1.35rem 1.25rem; }
}

.deck .card {
  background: var(--fog);
  border-radius: 10px;
  padding: 0.7rem 0.85rem;
  border: 1px solid var(--line);
}
.deck .card.blue { background: var(--sky); border-color: #b8d0ee; }
.deck .card.teal { background: var(--teal-soft); border-color: #a8dfc0; }
.deck .card.amber { background: var(--amber-soft); border-color: #f0d48a; }
.deck .card.coral { background: var(--coral-soft); border-color: #f5b8b8; }
.deck .card .label {
  font-family: Outfit, sans-serif;
  font-size: 0.66rem; font-weight: 700; letter-spacing: 0.06em;
  text-transform: uppercase; color: var(--blue-bright); margin-bottom: 0.2rem;
}
.deck .card.teal .label { color: var(--teal); }
.deck .card.amber .label { color: var(--amber); }
.deck .card.coral .label { color: var(--coral); }
.deck .card .value {
  font-family: Outfit, "Noto Sans SC", sans-serif;
  font-size: 0.98rem; font-weight: 700; color: var(--ink); margin-bottom: 0.15rem;
}
.deck .card p { margin: 0; font-size: 0.8rem; color: var(--ink-soft); line-height: 1.4; }

.deck .quote {
  background: var(--sky);
  border-left: 4px solid var(--blue-bright);
  border-radius: 0 10px 10px 0;
  padding: 0.65rem 1rem;
  font-size: 0.95rem; font-weight: 500; color: var(--ink);
  margin: 0.5rem 0;
}

.deck .flow {
  display: flex; flex-wrap: wrap; align-items: center; gap: 0.35rem;
  margin: 0.45rem 0 0.15rem;
}
.deck .flow-step {
  background: var(--ink); color: #fff;
  font-size: 0.78rem; font-weight: 600;
  padding: 0.35rem 0.65rem; border-radius: 7px;
}
.deck .flow-arrow { color: var(--blue-bright); font-weight: 800; font-size: 1rem; }

.deck ul.clean {
  list-style: none; padding: 0; margin: 0.25rem 0 0;
}
.deck ul.clean li {
  position: relative; padding: 0.2rem 0 0.2rem 1.05rem;
  font-size: 0.86rem;
}
.deck ul.clean li::before {
  content: ""; position: absolute; left: 0; top: 0.55rem;
  width: 6px; height: 6px; border-radius: 50%; background: var(--blue-bright);
}

.deck table.deck-table {
  width: 100%; border-collapse: collapse; font-size: 0.8rem;
  margin: 0.35rem 0 0;
}
.deck table.deck-table th {
  text-align: left; background: var(--ink); color: #fff;
  padding: 0.38rem 0.6rem; font-weight: 600;
}
.deck table.deck-table td {
  padding: 0.35rem 0.6rem; border-bottom: 1px solid var(--line);
  vertical-align: top;
}
.deck table.deck-table tr:nth-child(even) td { background: var(--fog); }

.deck .tag-row { display: flex; flex-wrap: wrap; gap: 0.35rem; margin-top: 0.4rem; }
.deck .tag {
  font-size: 0.72rem; font-weight: 600;
  padding: 0.2rem 0.5rem; border-radius: 6px;
  background: var(--sky); color: var(--blue);
}
.deck .tag.teal { background: var(--teal-soft); color: var(--teal); }
.deck .tag.amber { background: var(--amber-soft); color: var(--amber); }
.deck .tag.coral { background: var(--coral-soft); color: var(--coral); }

.deck .round-strip {
  display: grid; grid-template-columns: repeat(4, 1fr); gap: 0.45rem;
  margin-top: 0.4rem;
}
@media (max-width: 800px) { .deck .round-strip { grid-template-columns: 1fr 1fr; } }
.deck .round {
  border-radius: 10px; padding: 0.65rem 0.6rem; color: #fff; text-align: center;
}
.deck .round .r { font-family: Outfit, sans-serif; font-size: 0.68rem; font-weight: 700; opacity: 0.85; }
.deck .round .t { font-weight: 700; font-size: 0.9rem; margin: 0.12rem 0; }
.deck .round .d { font-size: 0.7rem; opacity: 0.9; line-height: 1.3; }
.deck .r1 { background: #1e5a96; }
.deck .r2 { background: #0f6e56; }
.deck .r3 { background: #7a5c00; }
.deck .r4 { background: #9b2c2c; }

.deck .close-line {
  font-family: Outfit, "Noto Sans SC", sans-serif;
  font-size: 1.05rem; font-weight: 700; color: #fff;
  margin: 0.25rem 0 0;
  line-height: 1.4;
}

/* 宽屏：把「标题区 + 内容区」压成更扁的横向构图 */
@media (min-width: 1100px) {
  .deck .slide.split-wide > .slide-body {
    display: grid;
    grid-template-columns: minmax(220px, 0.9fr) minmax(0, 1.6fr);
    gap: 0.75rem 1.5rem;
    align-items: start;
  }
  .deck .slide.split-wide .slide-num,
  .deck .slide.split-wide .slide-title {
    grid-column: 1;
  }
  .deck .slide.split-wide .slide-title { margin-bottom: 0; }
  .deck .slide.split-wide .slide-main {
    grid-column: 2;
    grid-row: 1 / span 8;
  }
  .deck .slide.stack-side > .slide-body > .after-lead {
    display: grid;
    grid-template-columns: 1.2fr 1fr;
    gap: 0.75rem 1.25rem;
    align-items: start;
  }
}

.deck-nav {
  position: sticky; top: 0; z-index: 40;
  display: flex; gap: 0.28rem; flex-wrap: wrap;
  background: rgba(255,255,255,0.92);
  backdrop-filter: blur(8px);
  border: 1px solid var(--line);
  border-radius: 10px;
  padding: 0.35rem 0.45rem;
  margin-bottom: 0.65rem;
  box-shadow: 0 3px 12px rgba(15,39,68,0.07);
}
.deck-nav a {
  font-size: 0.66rem; font-weight: 600; text-decoration: none;
  color: var(--ink-soft); padding: 0.22rem 0.42rem; border-radius: 5px;
  background: var(--fog);
}
.deck-nav a:hover { background: var(--sky); color: var(--blue); }

/* 收束页：单栏恢复 */
.deck .hero#s13 .slide-body,
.deck #s13.hero .slide-body {
  grid-template-columns: 1fr;
  max-width: 52rem;
}
</style>

<div class="deck" id="deck">

<nav class="deck-nav" aria-label="幻灯导航">
  <a href="#s0">封面</a>
  <a href="#s1">课程场景</a>
  <a href="#s2">知识技能</a>
  <a href="#s3">玩法</a>
  <a href="#s4">目标挑战</a>
  <a href="#s5">形态操控</a>
  <a href="#s6">推进</a>
  <a href="#s7">知识点</a>
  <a href="#s8">LLM</a>
  <a href="#s9">挑战A</a>
  <a href="#s10">挑战B</a>
  <a href="#s11">评估</a>
  <a href="#s12">帮助剧情</a>
  <a href="#s13">收束</a>
</nav>

<!-- 0 封面 -->
<section class="slide hero" id="s0">
  <div class="slide-body">
    <div class="eyebrow">AI 赋能教育游戏设计工作坊 · 约 10 分钟</div>
    <div>
      <h1>本地化商业模拟<br>Localization Business Simulation</h1>
      <p class="lede">用四轮网页决策沙盘，让翻译专业学生「做一遍 PM」——看见每一个早期选择如何变成后期的筹码或代价。</p>
    </div>
    <div class="hero-meta">
      <span class="chip solid">课程：《本地化翻译》</span>
      <span class="chip">场景：本地化项目管理</span>
      <span class="chip">形态：2D 网页模拟</span>
      <span class="chip">框架：16 步任务要求</span>
    </div>
  </div>
</section>

<!-- 1 课程 / 场景 / 目标 -->
<section class="slide stack-side" id="s1">
  <div class="slide-bar"></div>
  <div class="slide-body">
    <div class="slide-num"><span>01–03</span> 课程 · 场景 · 目标</div>
    <h2 class="slide-title">从「听一遍 PM」到「做一遍 PM」</h2>
    <div class="grid-3">
      <div class="card blue">
        <div class="label">课程</div>
        <div class="value">《本地化翻译》</div>
        <p>可嵌入《人工智能 + X》翻译模块第 6–9 节；面向英语学院翻译系。</p>
      </div>
      <div class="card teal">
        <div class="label">应用场景</div>
        <div class="value">本地化项目管理</div>
        <p>学生扮演 LSP 项目经理，承接游戏出海英语本地化全案。</p>
      </div>
      <div class="card amber">
        <div class="label">一句话目标</div>
        <div class="value">熟悉干系人 · 流程 · 决策点</div>
        <p>以及决策如何影响质量、成本与客户关系。</p>
      </div>
    </div>
    <div class="after-lead">
      <div>
        <h3>项目硬约束（情景沙箱）</h3>
        <div class="grid-2">
          <div class="card">
            <div class="label">客户 × LSP</div>
            <p><strong>米兔互娱</strong>（客户）委托 <strong>星桥语言科技</strong>（学生小组）完成《星际侦探》简中 → 美式英语本地化。</p>
          </div>
          <div class="card">
            <div class="label">规模与约束</div>
            <p>约 <strong>143,000 字</strong> · 工期 <strong>8 周</strong> · 预算 <strong>¥150,000</strong> · 「不接受明显机翻感」· 必须建术语库。</p>
          </div>
        </div>
      </div>
      <ul class="clean">
        <li><strong>干系人</strong>：客户 PM、译者、审校、工程师、QA、法务……诉求彼此冲突</li>
        <li><strong>核心要素</strong>：范围 / 进度 / 成本铁三角 + 质量、资产、合规</li>
        <li><strong>因果链</strong>：早期决策跨轮传导至后期谈判筹码与危机处置能力</li>
      </ul>
    </div>
  </div>
</section>

<!-- 2 知识技能 -->
<section class="slide stack-side" id="s2">
  <div class="slide-bar teal"></div>
  <div class="slide-body">
    <div class="slide-num"><span>04</span> 知识结构与技能体系</div>
    <h2 class="slide-title">四课闭环 = 游戏四轮</h2>
    <div class="round-strip">
      <div class="round r1"><div class="r">R1 · 第六节</div><div class="t">项目启动</div><div class="d">铁三角 · Kick-off · MT 策略</div></div>
      <div class="round r2"><div class="r">R2 · 第七节</div><div class="t">质量管控</div><div class="d">MQM · LQA · LQS</div></div>
      <div class="round r3"><div class="r">R3 · 第八节</div><div class="t">资产管理</div><div class="d">TM · 术语库 · ROI</div></div>
      <div class="round r4"><div class="r">R4 · 第九节</div><div class="t">风险应对</div><div class="d">SOP · 三危机 · 合规</div></div>
    </div>
    <div class="after-lead">
      <div>
        <h3>技能五维</h3>
        <div class="tag-row">
          <span class="tag">管理：范围 / 预算 / CCM</span>
          <span class="tag teal">质量：MQM / 抽样 / 阈值</span>
          <span class="tag amber">资产：清洗 / 匹配率 / 报价</span>
          <span class="tag coral">风险：登记册 / 备选资源</span>
          <span class="tag">AI 素养：批判性使用 MT/LLM</span>
        </div>
      </div>
      <div>
        <h3>游戏产出 ↔ 课程交付物</h3>
        <table class="deck-table">
          <thead><tr><th>轮次</th><th>游戏决策产出</th><th>课堂交付物</th></tr></thead>
          <tbody>
            <tr><td>R1</td><td>启动方案 / 决策摘要</td><td>项目启动简报</td></tr>
            <tr><td>R2</td><td>整改方案 / LQA 策略</td><td>质量验收标准 + LQA 样本</td></tr>
            <tr><td>R3</td><td>复用与报价方案</td><td>术语表 + 复用率测算</td></tr>
            <tr><td>R4</td><td>三危机应对摘要</td><td>SOP + 风险登记册</td></tr>
          </tbody>
        </table>
      </div>
    </div>
  </div>
</section>

<!-- 3 宏观行为 -->
<section class="slide" id="s3">
  <div class="slide-bar"></div>
  <div class="slide-body">
    <div class="slide-num"><span>05</span> 宏观游戏行为</div>
    <h2 class="slide-title">邮件驱动的决策循环</h2>
    <div class="quote">配置参数 → 观察铁三角与风险仪表 → 提交决策摘要 → <strong>带着后果进入下一轮</strong></div>
    <div class="grid-2" style="margin-top:0.45rem; align-items:stretch">
      <div>
        <div class="flow">
          <span class="flow-step">① 读邮件</span><span class="flow-arrow">→</span>
          <span class="flow-step">② 看状态</span><span class="flow-arrow">→</span>
          <span class="flow-step">③ 做决策</span><span class="flow-arrow">→</span>
          <span class="flow-step">④ 看后果</span><span class="flow-arrow">→</span>
          <span class="flow-step">⑤ 交摘要</span>
        </div>
      </div>
      <div class="card blue">
        <div class="label">核心设计原则</div>
        <div class="value">决策有代价，代价可跨轮传导</div>
        <p>Consequence Chain —— 不是单关闯关，而是一条因果链。</p>
      </div>
    </div>
  </div>
</section>

<!-- 4 目标与挑战形式 -->
<section class="slide" id="s4">
  <div class="slide-bar amber"></div>
  <div class="slide-body">
    <div class="slide-num"><span>06–07</span> 目标形式 · 挑战形式</div>
    <h2 class="slide-title">没有完美解，只有可解释的权衡</h2>
    <div class="grid-2">
      <div>
        <h3>目标怎么呈现</h3>
        <ul class="clean">
          <li>状态栏 KPI：预算 / 质量 / 工期 / 满意度</li>
          <li>铁三角绿·黄·红警示</li>
          <li>差异化后果卡（进入下一轮）</li>
          <li>决策摘要 = 通关凭证</li>
          <li>终局 PM 综合评分（/100）</li>
        </ul>
      </div>
      <div>
        <h3>挑战主要形态</h3>
        <ul class="clean">
          <li><strong>资源权衡</strong>：MT↑ → 省钱但机翻感↑</li>
          <li><strong>信息博弈</strong>：有无 LQS / 合同 → 谈判强弱</li>
          <li><strong>延迟后果</strong>：省下的 ¥3,000 → 后期数倍清洗</li>
          <li><strong>危机并发</strong>：人员 + 变更 + 合规同日爆发</li>
          <li><strong>社会沟通</strong>：主动披露 vs 回避数字</li>
        </ul>
      </div>
    </div>
    <div class="quote" style="margin-top:0.45rem">挑战不是打怪答题，而是<strong>在压力下做可辩护的商业决策</strong>。</div>
  </div>
</section>

<!-- 5 2D + 操控 -->
<section class="slide" id="s5">
  <div class="slide-bar"></div>
  <div class="slide-body">
    <div class="slide-num"><span>08–09</span> 形态 · 操控</div>
    <h2 class="slide-title">2D 网页模拟，课堂即开即用</h2>
    <div class="grid-2">
      <div class="card blue">
        <div class="label">为什么不是 3D</div>
        <div class="value">重点在决策逻辑</div>
        <p>HTML/CSS/JS 单页 · 加载快 · 易部署 · 适配桌面与窄屏。视觉：邮件卡 + 仪表盘 + 滑块决策区。</p>
      </div>
      <div class="card">
        <div class="label">基本操控</div>
        <p>鼠标点选策略 · 滑块调 MT/工期/折扣 · 步进器调人数 · 文本填小组名 · 密码门控节奏 · 一键复制摘要。</p>
      </div>
    </div>
  </div>
</section>

<!-- 6 推进 -->
<section class="slide" id="s6">
  <div class="slide-bar teal"></div>
  <div class="slide-body">
    <div class="slide-num"><span>10</span> 推进形式</div>
    <h2 class="slide-title">四轮线性 + 教师门控 + 状态继承</h2>
    <div class="flow">
      <span class="flow-step" style="background:#1e5a96">R1 启动</span><span class="flow-arrow">🔐</span>
      <span class="flow-step" style="background:#0f6e56">R2 质量</span><span class="flow-arrow">🔐</span>
      <span class="flow-step" style="background:#7a5c00">R3 资产</span><span class="flow-arrow">🔐</span>
      <span class="flow-step" style="background:#9b2c2c">R4 危机</span>
    </div>
    <p style="margin-top:0.45rem">前一轮决策写入 <code>localStorage</code>，后一轮读取并触发<strong>差异化剧本</strong>：</p>
    <div class="grid-2">
      <div class="card coral">
        <div class="label">高 MT 组</div>
        <p>进入「质量危机」邮件 · Critical 多 · 客户措辞强硬</p>
      </div>
      <div class="card amber">
        <div class="label">低 MT 组</div>
        <p>质量尚可，但进度缓冲耗尽 · 「修复不得超过 2 天」</p>
      </div>
    </div>
    <p style="margin-top:0.4rem;font-size:0.82rem;color:#64748b">同一课堂，多条路径 → 抽点时天然有对比样本。</p>
  </div>
</section>

<!-- 7 知识点展示 -->
<section class="slide" id="s7">
  <div class="slide-bar"></div>
  <div class="slide-body">
    <div class="slide-num"><span>11</span> 知识点展示讲解形式</div>
    <h2 class="slide-title">做中学：先感到疼/甜，再命名概念</h2>
    <div class="grid-3">
      <div class="card amber"><div class="label">情景邮件</div><p>客户语气抛出机翻感、续约、侵权</p></div>
      <div class="card blue"><div class="label">参数 Hint</div><p>控件旁短提示：成本、产能、后果</p></div>
      <div class="card teal"><div class="label">后果标签</div><p>「→ 决定第 N 轮样本难度」</p></div>
      <div class="card"><div class="label">动态仪表</div><p>铁三角 · ROI · 谈判态势</p></div>
      <div class="card"><div class="label">后果卡</div><p>解释「为什么你落在这个局面」</p></div>
      <div class="card"><div class="label">闭环反思表</div><p>今日危机 ← 哪一轮哪次决策</p></div>
    </div>
  </div>
</section>

<!-- 8 LLM -->
<section class="slide" id="s8">
  <div class="slide-bar amber"></div>
  <div class="slide-body">
    <div class="slide-num"><span>12</span> LLM 支撑的动态性</div>
    <h2 class="slide-title">规则引擎保公平，LLM 让情景「活」起来</h2>
    <p>当前版本以参数公式驱动；可扩展引入 LLM 的环节：</p>
    <table class="deck-table">
      <thead><tr><th>环节</th><th>动态性</th><th>教学价值</th></tr></thead>
      <tbody>
        <tr><td>情景邮件</td><td>按 MT/LQS 生成不同压力语气</td><td>干系人沟通真实感</td></tr>
        <tr><td>LQA 样本包</td><td>动态生成「机翻感」对话供标注</td><td>MQM 实操</td></tr>
        <tr><td>客户谈判 NPC</td><td>对学生文字回复作接受/追问</td><td>沟通策略迁移</td></tr>
        <tr><td>术语清洗助手</td><td>候选统一建议，学生批判采纳</td><td>AI 辅助 vs 把关</td></tr>
        <tr><td>风险参谋</td><td>给利弊草案，不给标准答案</td><td>批判性用 AI</td></tr>
      </tbody>
    </table>
    <div class="quote">边界：LLM 管情景与反馈动态化；<strong>评分与铁三角硬约束仍由规则引擎</strong>保证可复现。</div>
  </div>
</section>

<!-- 9 挑战 A -->
<section class="slide" id="s9">
  <div class="slide-bar"></div>
  <div class="slide-body">
    <div class="slide-num"><span>13A</span> 完整挑战 · 其一</div>
    <h2 class="slide-title">挑战 A：铁三角下的 MT 策略（R1）</h2>
    <div class="card amber" style="margin-bottom:0.5rem">
      <div class="label">情境</div>
      <p>143,000 字 · 8 周 · ¥150,000 · 「不接受机翻感」· 必须建术语库。今日提交启动方案。</p>
    </div>
    <div class="grid-3">
      <div class="card teal">
        <div class="label">低 MT &lt;30%</div>
        <div class="value">质量友好</div>
        <p>但工期缓冲极小 → R2「进度吃紧」剧本</p>
      </div>
      <div class="card coral">
        <div class="label">高 MT ≥60%</div>
        <div class="value">成本/工期松</div>
        <p>R2 高错误密度样本 · 客户暗示索赔</p>
      </div>
      <div class="card">
        <div class="label">不建术语库</div>
        <div class="value">省 ¥3,000</div>
        <p>违反 RFQ · R3 资产「混乱型」重罚</p>
      </div>
    </div>
    <p style="margin-top:0.45rem"><strong>学习目标：</strong>体验铁三角相互制约；理解 MT 不是开关，而是质量–成本–进度的连续权衡。</p>
  </div>
</section>

<!-- 10 挑战 B -->
<section class="slide stack-side" id="s10">
  <div class="slide-bar coral"></div>
  <div class="slide-body">
    <div class="slide-num"><span>13B</span> 完整挑战 · 其二</div>
    <h2 class="slide-title">挑战 B：三危机并发（R4）</h2>
    <div class="grid-3">
      <div class="card coral">
        <div class="label">情况一 · 人员</div>
        <div class="value">主译者住院</div>
        <p>~22,000 字未完成 · 剩余 3.5 周不可延误</p>
      </div>
      <div class="card amber">
        <div class="label">情况二 · 变更</div>
        <div class="value">追加 6,000 字</div>
        <p>客户要求：不加预算、不延期</p>
      </div>
      <div class="card" style="background:#f3eeff;border-color:#c8aaf0">
        <div class="label" style="color:#6a0dad">情况三 · 合规</div>
        <div class="value">版权侵权风险</div>
        <p>LSP 可能承担连带责任</p>
      </div>
    </div>
    <div class="after-lead">
      <div>
        <h3>跨轮因果（挑战完整性的关键）</h3>
        <table class="deck-table">
          <thead><tr><th>今日资源</th><th>来源决策</th></tr></thead>
          <tbody>
            <tr><td>替补到位成本 ¥1,500 / 5,500 / 13,000</td><td>R1 风险预案详细度</td></tr>
            <tr><td>变更谈判强势 / 一般 / 被动</td><td>R3 合同 CCM 条款</td></tr>
            <tr><td>紧急储备 ¥20,000 或 ¥12,000</td><td>R3 TM 折扣是否过激</td></tr>
            <tr><td>法务残余风险倍率</td><td>R1 是否有版权检查清单</td></tr>
          </tbody>
        </table>
      </div>
      <p style="margin-top:0.65rem"><strong>学习目标：</strong>理解「风险管理写在规划阶段」；在资源不足时做可辩护的优先级排序。</p>
    </div>
  </div>
</section>

<!-- 11 评估 -->
<section class="slide" id="s11">
  <div class="slide-bar teal"></div>
  <div class="slide-body">
    <div class="slide-num"><span>14</span> 学习效果采集与评估</div>
    <h2 class="slide-title">过程可追踪，路径可对比</h2>
    <div class="grid-2">
      <div class="card blue">
        <div class="label">采集什么</div>
        <ul class="clean">
          <li>每轮决策摘要（选项全记录）</li>
          <li>质量 / 预算 / 满意度轨迹</li>
          <li>差异化路径（高中低 MT 等）</li>
          <li>终局 PM 评分（规则引擎）</li>
          <li>抽点 + 交付物 + 反思报告</li>
        </ul>
      </div>
      <div class="card teal">
        <div class="label">如何判断掌握</div>
        <ul class="clean">
          <li>决策一致性：是否纠正前期短视</li>
          <li>概念迁移：能否用铁三角/MQM 解释</li>
          <li>因果意识：说得出「代价从哪来」</li>
          <li>AI 批判性：避免重蹈「纯 MT 救火」</li>
        </ul>
      </div>
    </div>
    <p style="margin-top:0.4rem;font-size:0.88rem">评估强调<strong>过程性与可解释性</strong>，不设唯一最优路径。</p>
  </div>
</section>

<!-- 12 帮助 + 剧情 -->
<section class="slide" id="s12">
  <div class="slide-bar amber"></div>
  <div class="slide-body">
    <div class="slide-num"><span>15–16</span> 帮助提示 · 风格剧情人物</div>
    <h2 class="slide-title">商务仿真世界里的帮助与沉浸</h2>
    <div class="grid-2">
      <div>
        <h3>帮助 / 提示</h3>
        <ul class="clean">
          <li>参数 Hint · 后果彩色标签</li>
          <li>铁三角 / 风险仪表诊断</li>
          <li>谈判态势（有无 LQS）</li>
          <li>R4 资源提示条：「你现有什么工具」</li>
          <li>原则：提示框架，不给标准答案</li>
        </ul>
      </div>
      <div>
        <h3>剧情弧线</h3>
        <div class="flow" style="margin-bottom:0.6rem">
          <span class="flow-step">立项</span><span class="flow-arrow">→</span>
          <span class="flow-step">质量投诉</span><span class="flow-arrow">→</span>
          <span class="flow-step">续集复约</span><span class="flow-arrow">→</span>
          <span class="flow-step">三危机</span><span class="flow-arrow">→</span>
          <span class="flow-step">闭环反思</span>
        </div>
        <p style="font-size:0.88rem"><strong>人物：</strong>张明（客户负责人）· 李玲（体验主管）· 主译者王磊 · 学生 = 星桥团队 · 教师 = 系统外导演</p>
      </div>
    </div>
    <div class="tag-row">
      <span class="tag">视觉：商务蓝仪表 + 邮件黄卡</span>
      <span class="tag coral">R4 红色危机强调</span>
      <span class="tag amber">4–5 人小组 · 教师门控</span>
    </div>
  </div>
</section>

<!-- 13 收束 -->
<section class="slide hero" id="s13">
  <div class="slide-body">
    <div class="eyebrow">收束</div>
    <h1 style="font-size:clamp(1.35rem, 2.8vw, 1.85rem); margin-bottom:1rem">因果链是核心玩法</h1>
    <p class="close-line">规则引擎保证因果可复现；LLM 可进一步让邮件、样本与谈判「活」起来——但判断，仍留给学生。</p>
    <p class="lede" style="margin-top:0.7rem; margin-bottom:0.55rem">本地化商业模拟：让翻译专业学生在出海项目里，亲手权衡质量–成本–工期，并看见每一个早期选择如何变成后期的筹码或代价。</p>
    <div class="hero-meta">
      <span class="chip solid">谢谢</span>
      <span class="chip">欢迎交流与试玩反馈</span>
    </div>
  </div>
</section>

</div>

<script>
(function () {
  var slides = Array.prototype.slice.call(document.querySelectorAll('#deck .slide'));
  if (!slides.length) return;
  function currentIndex() {
    var mid = window.scrollY + window.innerHeight * 0.28;
    var best = 0, bestDist = Infinity;
    slides.forEach(function (s, i) {
      var top = s.getBoundingClientRect().top + window.scrollY;
      var d = Math.abs(top - mid);
      if (d < bestDist) { bestDist = d; best = i; }
    });
    return best;
  }
  function go(delta) {
    var i = Math.min(slides.length - 1, Math.max(0, currentIndex() + delta));
    slides[i].scrollIntoView({ behavior: 'smooth', block: 'start' });
  }
  document.addEventListener('keydown', function (e) {
    var tag = (e.target && e.target.tagName) || '';
    if (tag === 'INPUT' || tag === 'TEXTAREA' || e.target.isContentEditable) return;
    if (e.key === 'ArrowDown' || e.key === 'PageDown' || (e.key === ' ' && !e.shiftKey)) {
      e.preventDefault(); go(1);
    } else if (e.key === 'ArrowUp' || e.key === 'PageUp' || (e.key === ' ' && e.shiftKey)) {
      e.preventDefault(); go(-1);
    }
  });
})();
</script>
