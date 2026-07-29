---
title: "本地化商业模拟 · 中文演示"
permalink: /talks/2026-07-28-zh/
layout: single
author_profile: false
sitemap: false
search: false
---


<style>
@import url('https://fonts.googleapis.com/css2?family=Outfit:wght@500;700;800&family=Noto+Sans+SC:wght@400;500;700&display=swap');

.masthead {
  padding-top: 0.35rem !important;
  padding-bottom: 0.35rem !important;
}
#main {
  max-width: min(1280px, 96vw) !important;
  margin-top: 0.35rem !important;
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
.page__content { padding-bottom: 0 !important; }

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
  --slide-gap: clamp(2.5rem, 12vh, 7rem);
  font-family: Outfit, "Noto Sans SC", "Segoe UI", sans-serif;
  color: var(--ink-soft);
  line-height: 1.45;
  width: 100%;
  max-width: min(1180px, 100%);
  margin: 0 auto 2rem;
}

.deck .slide {
  scroll-margin-top: 0.75rem;
  background: var(--white);
  border: 1px solid var(--line);
  border-radius: 16px;
  overflow: hidden;
  margin-bottom: var(--slide-gap);
  box-shadow: 0 8px 28px rgba(15, 39, 68, 0.06);
  min-height: calc(100dvh - 5.25rem);
  display: flex;
  flex-direction: column;
}

.deck .slide-bar {
  height: 6px; flex-shrink: 0;
  background: linear-gradient(90deg, var(--blue) 0%, #4a90c8 55%, #7eb8d8 100%);
}
.deck .slide-bar.teal { background: linear-gradient(90deg, #0f6e56, #3d9b7a); }
.deck .slide-bar.amber { background: linear-gradient(90deg, #9a6700, #d4a017); }
.deck .slide-bar.coral { background: linear-gradient(90deg, #b42318, #e05a4f); }

.deck .slide-body {
  flex: 1;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 1.6rem 2rem 1.75rem;
}

.deck .slide-num {
  display: inline-flex; align-items: center; gap: 0.45rem;
  font-size: 0.72rem; font-weight: 700; letter-spacing: 0.08em;
  text-transform: uppercase; color: var(--blue-bright);
  margin-bottom: 0.45rem;
}
.deck .slide-num span {
  background: var(--sky); color: var(--blue);
  border-radius: 999px; padding: 0.12rem 0.55rem;
}
.deck .slide-num .zh {
  font-family: "Noto Sans SC", sans-serif;
  font-weight: 500; letter-spacing: 0; text-transform: none;
  color: #64748b; font-size: 0.78rem;
}

.deck h2.slide-title {
  font-size: clamp(1.35rem, 2.4vw, 1.75rem);
  font-weight: 800; color: var(--ink);
  margin: 0 0 0.25rem; line-height: 1.2; border: none; padding: 0;
}
.deck .title-zh {
  font-family: "Noto Sans SC", sans-serif;
  font-size: 0.95rem; font-weight: 500; color: #64748b;
  margin: 0 0 1rem;
}
.deck h3 {
  font-size: 1rem; font-weight: 700; color: var(--ink);
  margin: 0.85rem 0 0.4rem; border: none; padding: 0;
}
.deck p { margin: 0 0 0.55rem; font-size: 1rem; }
.deck strong { color: var(--ink); font-weight: 700; }

.deck .hero {
  background:
    radial-gradient(ellipse 80% 60% at 100% 0%, rgba(44,107,172,0.18), transparent 55%),
    radial-gradient(ellipse 50% 40% at 0% 100%, rgba(15,110,86,0.12), transparent 50%),
    linear-gradient(160deg, #0f2744 0%, #1a3f6b 48%, #1e5a96 100%);
  color: #e8eef6;
  border: none;
}
.deck .hero .slide-body {
  padding: 2rem 2.25rem;
  justify-content: center;
}
.deck .hero .eyebrow {
  font-size: 0.78rem; font-weight: 700; letter-spacing: 0.1em;
  text-transform: uppercase; color: #9ec0e0; margin-bottom: 0.75rem;
}
.deck .hero .eyebrow .zh {
  display: block; margin-top: 0.25rem;
  font-family: "Noto Sans SC", sans-serif;
  letter-spacing: 0.04em; text-transform: none; font-weight: 500;
  color: #a8c4dc; font-size: 0.82rem;
}
.deck .hero h1 {
  font-size: clamp(1.7rem, 3.2vw, 2.45rem);
  font-weight: 800; color: #fff; margin: 0 0 0.2rem;
  line-height: 1.15; border: none;
}
.deck .hero .title-zh {
  color: #9ec0e0; font-size: 1.05rem; margin-bottom: 1rem;
}
.deck .hero .lede {
  font-size: 1.08rem; color: #c5d6e8; max-width: 38em; margin-bottom: 1.35rem;
}
.deck .hero-meta { display: flex; flex-wrap: wrap; gap: 0.45rem; }
.deck .chip {
  display: inline-block;
  background: rgba(255,255,255,0.12);
  border: 1px solid rgba(255,255,255,0.22);
  border-radius: 8px;
  padding: 0.35rem 0.75rem;
  font-size: 0.82rem; color: #e8eef6;
}
.deck .chip.solid {
  background: #fff; color: var(--blue); font-weight: 700; border-color: #fff;
}
.deck .hero-actions {
  display: flex; flex-wrap: wrap; gap: 0.65rem;
  margin-top: 1.35rem;
}
.deck .btn-deck {
  display: inline-flex; align-items: center; gap: 0.4rem;
  font-family: Outfit, "Noto Sans SC", sans-serif;
  font-size: 0.9rem; font-weight: 700; text-decoration: none;
  padding: 0.55rem 1.05rem; border-radius: 10px;
  border: 1px solid transparent;
  transition: transform 0.15s ease, background 0.15s ease;
}
.deck .btn-deck:hover { transform: translateY(-1px); text-decoration: none; }
.deck .btn-deck.primary {
  background: #fff; color: var(--blue); border-color: #fff;
}
.deck .btn-deck.primary:hover { background: #e8f1fa; color: var(--blue); }
.deck .btn-deck.ghost {
  background: rgba(255,255,255,0.1);
  color: #e8eef6;
  border-color: rgba(255,255,255,0.35);
}
.deck .btn-deck.ghost:hover { background: rgba(255,255,255,0.2); color: #fff; }

.deck .grid-2 {
  display: grid; grid-template-columns: 1fr 1fr; gap: 0.85rem;
}
.deck .grid-3 {
  display: grid; grid-template-columns: repeat(3, 1fr); gap: 0.75rem;
}
.deck .grid-4 {
  display: grid; grid-template-columns: repeat(4, 1fr); gap: 0.65rem;
}
@media (max-width: 800px) {
  .deck .grid-2, .deck .grid-3, .deck .grid-4 { grid-template-columns: 1fr; }
  .deck .slide { min-height: auto; }
  .deck .slide-body { justify-content: flex-start; padding: 1.25rem 1.2rem 1.4rem; }
}

.deck .card {
  background: var(--fog);
  border-radius: 12px;
  padding: 1rem 1.1rem;
  border: 1px solid var(--line);
}
.deck .card.blue { background: var(--sky); border-color: #b8d0ee; }
.deck .card.teal { background: var(--teal-soft); border-color: #a8dfc0; }
.deck .card.amber { background: var(--amber-soft); border-color: #f0d48a; }
.deck .card.coral { background: var(--coral-soft); border-color: #f5b8b8; }
.deck .card .label {
  font-size: 0.7rem; font-weight: 700; letter-spacing: 0.06em;
  text-transform: uppercase; color: var(--blue-bright); margin-bottom: 0.3rem;
}
.deck .card.teal .label { color: var(--teal); }
.deck .card.amber .label { color: var(--amber); }
.deck .card.coral .label { color: var(--coral); }
.deck .card .value {
  font-size: 1.08rem; font-weight: 700; color: var(--ink); margin-bottom: 0.3rem;
}
.deck .card p { margin: 0; font-size: 0.9rem; color: var(--ink-soft); line-height: 1.4; }

.deck .quote {
  background: var(--sky);
  border-left: 5px solid var(--blue-bright);
  border-radius: 0 12px 12px 0;
  padding: 0.9rem 1.2rem;
  font-size: 1.05rem; font-weight: 500; color: var(--ink);
  margin: 0.4rem 0 0;
}

.deck .flow {
  display: flex; flex-wrap: wrap; align-items: center; gap: 0.4rem;
  margin: 0.35rem 0;
}
.deck .flow-step {
  background: var(--ink); color: #fff;
  font-size: 0.88rem; font-weight: 600;
  padding: 0.5rem 0.85rem; border-radius: 8px;
}
.deck .flow-arrow { color: var(--blue-bright); font-weight: 800; font-size: 1.15rem; }

.deck ul.clean {
  list-style: none; padding: 0; margin: 0.2rem 0 0;
}
.deck ul.clean li {
  position: relative; padding: 0.35rem 0 0.35rem 1.15rem;
  font-size: 0.95rem;
}
.deck ul.clean li::before {
  content: ""; position: absolute; left: 0; top: 0.7rem;
  width: 7px; height: 7px; border-radius: 50%; background: var(--blue-bright);
}

.deck .round-strip {
  display: grid; grid-template-columns: repeat(4, 1fr); gap: 0.6rem;
}
@media (max-width: 800px) { .deck .round-strip { grid-template-columns: 1fr 1fr; } }
.deck .round {
  border-radius: 12px; padding: 1rem 0.75rem; color: #fff; text-align: center;
}
.deck .round .r { font-size: 0.72rem; font-weight: 700; opacity: 0.85; }
.deck .round .t { font-weight: 700; font-size: 1.02rem; margin: 0.25rem 0; }
.deck .round .d { font-size: 0.78rem; opacity: 0.92; line-height: 1.35; }
.deck .r1 { background: #1e5a96; }
.deck .r2 { background: #0f6e56; }
.deck .r3 { background: #7a5c00; }
.deck .r4 { background: #9b2c2c; }

.deck .close-line {
  font-size: 1.2rem; font-weight: 700; color: #fff;
  margin: 0.35rem 0 0; line-height: 1.45; max-width: 36em;
}

.deck-nav {
  position: sticky; top: 0; z-index: 40;
  display: flex; gap: 0.3rem; flex-wrap: wrap;
  background: rgba(255,255,255,0.94);
  backdrop-filter: blur(8px);
  border: 1px solid var(--line);
  border-radius: 12px;
  padding: 0.4rem 0.5rem;
  margin-bottom: 0.85rem;
  box-shadow: 0 4px 16px rgba(15,39,68,0.08);
}
.deck-nav a {
  font-size: 0.7rem; font-weight: 600; text-decoration: none;
  color: var(--ink-soft); padding: 0.28rem 0.48rem; border-radius: 6px;
  background: var(--fog);
}
.deck-nav a:hover { background: var(--sky); color: var(--blue); }

.deck #s13.hero .slide-body { max-width: 48rem; }
</style>

<div class="deck" id="deck">

<nav class="deck-nav" aria-label="幻灯导航">
  <a href="#s0">封面</a>
  <a href="#s1">想法</a>
  <a href="#s2">设定</a>
  <a href="#s3">四轮</a>
  <a href="#s4">玩法</a>
  <a href="#s5">权衡</a>
  <a href="#s6">形态</a>
  <a href="#s7">推进</a>
  <a href="#s8">学习</a>
  <a href="#s9">AI</a>
  <a href="#s10">示例A</a>
  <a href="#s11">示例B</a>
  <a href="#s12">评估</a>
  <a href="#s13">收束</a>
</nav>

<!-- 0 Cover -->
<section class="slide hero" id="s0">
  <div class="slide-body">
    <div class="eyebrow">
      AI 赋能教育游戏设计工作坊 · 约 10 分钟
      <span class="zh">AI-Powered Educational Game Design · ~10 min</span>
    </div>
    <h1>本地化商业模拟</h1>
    <p class="title-zh">Localization Business Simulation</p>
    <p class="lede">学生不是听一遍项目管理，而是<strong>亲手跑一遍</strong>游戏翻译项目——看见每个选择如何变成后来的筹码或代价。</p>
    <div class="hero-meta">
      <span class="chip solid">课程：本地化翻译</span>
      <span class="chip">网页决策游戏</span>
      <span class="chip">四轮 · 课堂即用</span>
    </div>
    <div class="hero-actions">
      <a class="btn-deck primary" href="https://chezvivian.github.io/class/localization-sim/" target="_blank" rel="noopener noreferrer">打开模拟平台 ↗</a>
      <a class="btn-deck ghost" href="/talks/2026-07-28">English</a>
    </div>
  </div>
</section>

<!-- 1 -->
<section class="slide" id="s1">
  <div class="slide-bar"></div>
  <div class="slide-body">
    <div class="slide-num"><span>01</span> 核心想法</div>
    <h2 class="slide-title">从「听一遍」到「做一遍」</h2>
    <div class="grid-3">
      <div class="card blue">
        <div class="label">对象</div>
        <div class="value">翻译专业学生</div>
        <p>他们很快会面对跨境内容、客户与紧迫工期。</p>
      </div>
      <div class="card teal">
        <div class="label">游戏中的角色</div>
        <div class="value">项目经理</div>
        <p>游戏公司请他们的团队，把一款游戏译成英语。</p>
      </div>
      <div class="card amber">
        <div class="label">学习目标</div>
        <div class="value">看见选择的分量</div>
        <p>质量、成本、时间、客户信任，常常相互拉扯。</p>
      </div>
    </div>
  </div>
</section>

<!-- 2 -->
<section class="slide" id="s2">
  <div class="slide-bar teal"></div>
  <div class="slide-body">
    <div class="slide-num"><span>02</span> 故事设定</div>
    <h2 class="slide-title">一个项目，边界清楚</h2>
    <div class="grid-2">
      <div class="card">
        <div class="label">任务</div>
        <p>把一款中文游戏译成美式英语，准备海外上线。</p>
      </div>
      <div class="card">
        <div class="label">硬约束</div>
        <p>约 <strong>143,000 字</strong> · <strong>8 周</strong> · 预算 <strong>¥150,000</strong> · 不能有明显「机翻感」。</p>
      </div>
    </div>
    <div class="quote">很多人想要不同的东西。学生必须做决定——并承担结果。</div>
  </div>
</section>

<!-- 3 -->
<section class="slide" id="s3">
  <div class="slide-bar"></div>
  <div class="slide-body">
    <div class="slide-num"><span>03</span> 课程即游戏</div>
    <h2 class="slide-title">四节课 = 游戏四轮</h2>
    <div class="round-strip">
      <div class="round r1"><div class="r">第一轮</div><div class="t">启动项目</div><div class="d">规划人力、时间、预算与工具</div></div>
      <div class="round r2"><div class="r">第二轮</div><div class="t">守住质量</div><div class="d">检查问题并整改</div></div>
      <div class="round r3"><div class="r">第三轮</div><div class="t">复用资产</div><div class="d">用旧译文与术语省时间</div></div>
      <div class="round r4"><div class="r">第四轮</div><div class="t">应对危机</div><div class="d">人员、变更、合规风险</div></div>
    </div>
  </div>
</section>

<!-- 4 -->
<section class="slide" id="s4">
  <div class="slide-bar amber"></div>
  <div class="slide-body">
    <div class="slide-num"><span>04</span> 怎么玩</div>
    <h2 class="slide-title">读邮件 → 做决定 → 承担后果</h2>
    <div class="flow">
      <span class="flow-step">1. 读客户邮件</span><span class="flow-arrow">→</span>
      <span class="flow-step">2. 看仪表盘</span><span class="flow-arrow">→</span>
      <span class="flow-step">3. 做出选择</span><span class="flow-arrow">→</span>
      <span class="flow-step">4. 看局面如何变</span>
    </div>
    <div class="quote">每个选择都有代价。这个代价可能跟到后面几轮。</div>
  </div>
</section>

<!-- 5 -->
<section class="slide" id="s5">
  <div class="slide-bar"></div>
  <div class="slide-body">
    <div class="slide-num"><span>05</span> 目标与挑战</div>
    <h2 class="slide-title">没有完美解，只有说得通的权衡</h2>
    <div class="grid-2">
      <div class="card blue">
        <div class="label">学生盯着什么</div>
        <ul class="clean">
          <li>预算、质量、工期、客户满意度</li>
          <li>绿 / 黄 / 红警示</li>
          <li>每轮写一份短决策摘要</li>
        </ul>
      </div>
      <div class="card amber">
        <div class="label">难在哪里</div>
        <ul class="clean">
          <li>现在省钱，后面可能更贵</li>
          <li>求快可能伤质量</li>
          <li>好几件坏事可能一起砸来</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<!-- 6 -->
<section class="slide" id="s6">
  <div class="slide-bar teal"></div>
  <div class="slide-body">
    <div class="slide-num"><span>06</span> 形态与操控</div>
    <h2 class="slide-title">简单网页，课堂即开即用</h2>
    <div class="grid-2">
      <div class="card blue">
        <div class="label">为什么不是 3D？</div>
        <div class="value">重点在决策</div>
        <p>加载快、好分享，教室电脑也能顺畅打开。</p>
      </div>
      <div class="card">
        <div class="label">学生怎么操作</div>
        <p>点选方案 · 拖动滑块 · 写小组备注 · 教师用密码解锁下一轮。</p>
      </div>
    </div>
  </div>
</section>

<!-- 7 -->
<section class="slide" id="s7">
  <div class="slide-bar"></div>
  <div class="slide-body">
    <div class="slide-num"><span>07</span> 推进方式</div>
    <h2 class="slide-title">上一轮的选择，改写下一轮的剧本</h2>
    <div class="flow">
      <span class="flow-step" style="background:#1e5a96">启动</span><span class="flow-arrow">🔐</span>
      <span class="flow-step" style="background:#0f6e56">质量</span><span class="flow-arrow">🔐</span>
      <span class="flow-step" style="background:#7a5c00">资产</span><span class="flow-arrow">🔐</span>
      <span class="flow-step" style="background:#9b2c2c">危机</span>
    </div>
    <div class="grid-2" style="margin-top:0.85rem">
      <div class="card coral">
        <div class="label">如果机器翻译用得太多</div>
        <p>客户会很生气。错误更多。后面更难收拾。</p>
      </div>
      <div class="card amber">
        <div class="label">如果特别慢、特别仔细</div>
        <p>质量更好——但几乎没留下修复时间。</p>
      </div>
    </div>
  </div>
</section>

<!-- 8 -->
<section class="slide" id="s8">
  <div class="slide-bar amber"></div>
  <div class="slide-body">
    <div class="slide-num"><span>08</span> 知识点怎么进来</div>
    <h2 class="slide-title">先体验痛点，再给概念名字</h2>
    <div class="grid-3">
      <div class="card amber"><div class="label">情景邮件</div><p>客户语气本身就在传达压力与利害。</p></div>
      <div class="card blue"><div class="label">短提示</div><p>每个控件旁边用白话说明成本与风险。</p></div>
      <div class="card teal"><div class="label">后果卡</div><p>「之所以落到这一步，是因为你之前的选择。」</p></div>
    </div>
  </div>
</section>

<!-- 9 -->
<section class="slide" id="s9">
  <div class="slide-bar"></div>
  <div class="slide-body">
    <div class="slide-num"><span>09</span> AI 扮演什么角色</div>
    <h2 class="slide-title">规则保证公平；AI 让情景更生动</h2>
    <div class="grid-2">
      <div class="card teal">
        <div class="label">规则引擎</div>
        <div class="value">分数与硬约束</div>
        <p>相同输入 → 相同结果。打分公平可复现。</p>
      </div>
      <div class="card blue">
        <div class="label">大语言模型（可选）</div>
        <div class="value">邮件、样本、回复</div>
        <p>压力与变化更自然——但不直接给「标准答案」。</p>
      </div>
    </div>
    <div class="quote">AI 帮忙讲故事。判断，仍留给学生。</div>
  </div>
</section>

<!-- 10 -->
<section class="slide" id="s10">
  <div class="slide-bar coral"></div>
  <div class="slide-body">
    <div class="slide-num"><span>10</span> 挑战示例 A</div>
    <h2 class="slide-title">你会用多少机器翻译？</h2>
    <div class="grid-3">
      <div class="card teal">
        <div class="label">用得少</div>
        <div class="value">质量更稳</div>
        <p>但后面几乎没有缓冲时间。</p>
      </div>
      <div class="card coral">
        <div class="label">用得多</div>
        <div class="value">更省钱、更快</div>
        <p>下一轮客户可能严厉投诉。</p>
      </div>
      <div class="card amber">
        <div class="label">不建术语表</div>
        <div class="value">眼下省一点钱</div>
        <p>后面复用文本时容易一团乱。</p>
      </div>
    </div>
  </div>
</section>

<!-- 11 -->
<section class="slide" id="s11">
  <div class="slide-bar amber"></div>
  <div class="slide-body">
    <div class="slide-num"><span>11</span> 挑战示例 B</div>
    <h2 class="slide-title">三件事同一天砸过来</h2>
    <div class="grid-3">
      <div class="card coral">
        <div class="label">人员</div>
        <div class="value">主译者生病</div>
        <p>工作没做完。截止日期不能动。</p>
      </div>
      <div class="card amber">
        <div class="label">变更</div>
        <div class="value">客户追加文本</div>
        <p>不加钱，也不延期。</p>
      </div>
      <div class="card blue">
        <div class="label">合规</div>
        <div class="value">版权风险</div>
        <p>他们的公司可能要一起承担责任。</p>
      </div>
    </div>
    <div class="quote">早期规划，会变成今天手里真正能用的工具。</div>
  </div>
</section>

<!-- 12 -->
<section class="slide" id="s12">
  <div class="slide-bar teal"></div>
  <div class="slide-body">
    <div class="slide-num"><span>12</span> 如何评估</div>
    <h2 class="slide-title">评的是思考过程，不是唯一标准答案</h2>
    <div class="grid-2">
      <div class="card blue">
        <div class="label">采集什么</div>
        <ul class="clean">
          <li>每轮的决策</li>
          <li>预算 / 质量 / 信任如何变化</li>
          <li>结束时的短反思</li>
        </ul>
      </div>
      <div class="card teal">
        <div class="label">什么叫「学得好」</div>
        <ul class="clean">
          <li>能说清为什么这样选</li>
          <li>能把今天的痛连回早先的选择</li>
          <li>把 AI 当助手，而不是盲目自动驾驶</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<!-- 13 -->
<section class="slide hero" id="s13">
  <div class="slide-body">
    <div class="eyebrow">
      收束
      <span class="zh">Takeaway</span>
    </div>
    <h1>因果链，就是核心玩法</h1>
    <p class="title-zh">Cause and effect is the gameplay</p>
    <p class="close-line">规则让结果公平可复现；AI 可以让故事更生动；判断，仍留给学生。</p>
    <div class="hero-meta" style="margin-top:1.25rem">
      <span class="chip solid">谢谢</span>
      <span class="chip">欢迎提问与试玩反馈</span>
    </div>
  </div>
</section>

</div>

<script>
(function () {
  var slides = Array.prototype.slice.call(document.querySelectorAll('#deck .slide'));
  if (!slides.length) return;
  function currentIndex() {
    var mid = window.scrollY + window.innerHeight * 0.35;
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
    if (e.key === 'ArrowDown' || e.key === 'PageDown' || e.key === 'ArrowRight' || (e.key === ' ' && !e.shiftKey)) {
      e.preventDefault(); go(1);
    } else if (e.key === 'ArrowUp' || e.key === 'PageUp' || e.key === 'ArrowLeft' || (e.key === ' ' && e.shiftKey)) {
      e.preventDefault(); go(-1);
    }
  });
})();
</script>
