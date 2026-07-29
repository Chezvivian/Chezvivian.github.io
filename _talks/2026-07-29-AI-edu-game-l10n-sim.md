---
title: "2026-07-29 Localization Business Simulation · 本地化商业模拟"
collection: talks
type: "Talk"
permalink: talks/2026-07-29
venue: "AI-Empowered Education Forum / Educational Game Design Workshop · 人工智能赋能教育学术交流会"
date: 2026-07-29
location: "Beijing"
author_profile: false
classes: wide
excerpt: "A walkthrough of an AI-supported educational game that lets translation students manage a game localization project through decisions and consequences."
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

<nav class="deck-nav" aria-label="Slide navigation">
  <a href="#s0">Cover</a>
  <a href="#s1">Idea</a>
  <a href="#s2">World</a>
  <a href="#s3">4 Rounds</a>
  <a href="#s4">Play</a>
  <a href="#s5">Tradeoffs</a>
  <a href="#s6">Form</a>
  <a href="#s7">Carryover</a>
  <a href="#s8">Learning</a>
  <a href="#s9">AI</a>
  <a href="#s10">Example A</a>
  <a href="#s11">Example B</a>
  <a href="#s12">Assessment</a>
  <a href="#s13">Close</a>
</nav>

<!-- 0 Cover -->
<section class="slide hero" id="s0">
  <div class="slide-body">
    <div class="eyebrow">
      AI-Powered Educational Game Design
      <span class="zh">AI 赋能教育游戏设计工作坊</span>
    </div>
    <h1>Localization Business Simulation</h1>
    <p class="title-zh">本地化商业模拟</p>
    <p class="lede">Students learn project management by <strong>running</strong> a game translation project—not by listening to a lecture about it.</p>
    <div class="hero-meta">
      <span class="chip solid">Course: Localization Translation</span>
      <span class="chip">Web-based decision game</span>
      <span class="chip">4 rounds · classroom ready</span>
    </div>
    <div class="hero-actions">
      <a class="btn-deck primary" href="https://chezvivian.github.io/class/localization-sim/" target="_blank" rel="noopener noreferrer">Open the simulation ↗</a>
      <a class="btn-deck ghost" href="/talks/2026-07-28-zh/">中文演示</a>
    </div>
  </div>
</section>

<!-- 1 Core idea -->
<section class="slide" id="s1">
  <div class="slide-bar"></div>
  <div class="slide-body">
    <div class="slide-num"><span>01</span> The big idea <span class="zh">核心思路</span></div>
    <h2 class="slide-title">From hearing about the job → doing the job</h2>
    <p class="title-zh">从听课到角色扮演</p>
    <div class="grid-3">
      <div class="card blue">
        <div class="label">Who</div>
        <div class="value">Translation students</div>
        <p>They will soon work with global content, clients, and tight deadlines.</p>
      </div>
      <div class="card teal">
        <div class="label">Role in the game</div>
        <div class="value">Project manager</div>
        <p>A game studio hires their team to translate a game into English.</p>
      </div>
      <div class="card amber">
        <div class="label">Learning goal</div>
        <div class="value">See how choices matter</div>
        <p>Quality, cost, time, and client trust all pull in different directions.</p>
      </div>
    </div>
  </div>
</section>

<!-- 2 Scenario -->
<section class="slide" id="s2">
  <div class="slide-bar teal"></div>
  <div class="slide-body">
    <div class="slide-num"><span>02</span> The story world <span class="zh">故事设定</span></div>
    <h2 class="slide-title">One project. Clear limits.</h2>
    <p class="title-zh">一个本地化翻译项目：任务、团队、成本清晰</p>
    <div class="grid-2">
      <div class="card">
        <div class="label">The job</div>
        <p>Translate a Chinese game into American English for an overseas launch.</p>
      </div>
      <div class="card">
        <div class="label">The limits</div>
        <p><strong>~143,000 words</strong> · <strong>8 weeks</strong> · <strong>¥150,000</strong> budget · quality must not feel “machine-translated”.</p>
      </div>
    </div>
    <div class="quote">Many people want different things. Students must decide—and live with the result.</div>
  </div>
</section>

<!-- 3 Four rounds -->
<section class="slide" id="s3">
  <div class="slide-bar"></div>
  <div class="slide-body">
    <div class="slide-num"><span>03</span> Course = game <span class="zh">课程即游戏</span></div>
    <h2 class="slide-title">Four lessons → four rounds</h2>
    <p class="title-zh">四节课 = 游戏四轮</p>
    <div class="round-strip">
      <div class="round r1"><div class="r">Round 1</div><div class="t">Start the project</div><div class="d">Plan people, time, money, and tools</div></div>
      <div class="round r2"><div class="r">Round 2</div><div class="t">Protect quality</div><div class="d">Check work and fix problems</div></div>
      <div class="round r3"><div class="r">Round 3</div><div class="t">Reuse assets</div><div class="d">Save time with past work &amp; terms</div></div>
      <div class="round r4"><div class="r">Round 4</div><div class="t">Handle crises</div><div class="d">People, change requests, legal risk</div></div>
    </div>
  </div>
</section>

<!-- 4 How you play -->
<section class="slide" id="s4">
  <div class="slide-bar amber"></div>
  <div class="slide-body">
    <div class="slide-num"><span>04</span> How you play <span class="zh">怎么玩</span></div>
    <h2 class="slide-title">Read mail → decide → face the result</h2>
    <p class="title-zh">读邮件 → 做决定 → 承担后果</p>
    <div class="flow">
      <span class="flow-step">1. Read the client email</span><span class="flow-arrow">→</span>
      <span class="flow-step">2. Check the dashboard</span><span class="flow-arrow">→</span>
      <span class="flow-step">3. Make a choice</span><span class="flow-arrow">→</span>
      <span class="flow-step">4. See what changes</span>
    </div>
    <div class="quote">Every choice has a cost. That cost can follow you into later rounds.</div>
  </div>
</section>

<!-- 5 Tradeoffs -->
<section class="slide" id="s5">
  <div class="slide-bar"></div>
  <div class="slide-body">
    <div class="slide-num"><span>05</span> Goals &amp; challenges <span class="zh">目标与挑战</span></div>
    <h2 class="slide-title">No perfect answer—only a defendable one</h2>
    <p class="title-zh">没有完美的答案，只有合理的权衡</p>
    <div class="grid-2">
      <div class="card blue">
        <div class="label">What students watch</div>
        <ul class="clean">
          <li>Budget, quality, deadline, client happiness</li>
          <li>Green / yellow / red warnings</li>
          <li>A short written decision summary each round</li>
        </ul>
      </div>
      <div class="card amber">
        <div class="label">What makes it hard</div>
        <ul class="clean">
          <li>Cheap now may cost more later</li>
          <li>Speed can hurt quality</li>
          <li>Several problems can hit at once</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<!-- 6 Form -->
<section class="slide" id="s6">
  <div class="slide-bar teal"></div>
  <div class="slide-body">
    <div class="slide-num"><span>06</span> Form &amp; controls <span class="zh">游戏的形式</span></div>
    <h2 class="slide-title">A simple web page—open and play</h2>
    <p class="title-zh">简单网页，课堂即开即用</p>
    <div class="grid-2">
      <div class="card blue">
        <div class="label">Why not 3D?</div>
        <div class="value">Focus on decisions</div>
        <p>Fast to load, easy to share, works on classroom computers.</p>
      </div>
      <div class="card">
        <div class="label">How students interact</div>
        <p>Click options · move sliders · write a short team note · teacher unlocks the next round with a password.</p>
      </div>
    </div>
  </div>
</section>

<!-- 7 Carryover -->
<section class="slide" id="s7">
  <div class="slide-bar"></div>
  <div class="slide-body">
    <div class="slide-num"><span>07</span> Progress <span class="zh">推进方式</span></div>
    <h2 class="slide-title">Your past choices change the next story</h2>
    <p class="title-zh">上一轮的选择，改写下一轮的剧本</p>
    <div class="flow">
      <span class="flow-step" style="background:#1e5a96">Start</span><span class="flow-arrow">🔐</span>
      <span class="flow-step" style="background:#0f6e56">Quality</span><span class="flow-arrow">🔐</span>
      <span class="flow-step" style="background:#7a5c00">Assets</span><span class="flow-arrow">🔐</span>
      <span class="flow-step" style="background:#9b2c2c">Crisis</span>
    </div>
    <div class="grid-2" style="margin-top:0.85rem">
      <div class="card coral">
        <div class="label">If they overused machine translation</div>
        <p>The client returns angry. More errors. Harder recovery.</p>
      </div>
      <div class="card amber">
        <div class="label">If they went very slow &amp; careful</div>
        <p>Quality is better—but almost no time left to fix anything.</p>
      </div>
    </div>
  </div>
</section>

<!-- 8 Learning -->
<section class="slide" id="s8">
  <div class="slide-bar amber"></div>
  <div class="slide-body">
    <div class="slide-num"><span>08</span> How learning happens <span class="zh">知识点怎么进来</span></div>
    <h2 class="slide-title">Feel it first. Name it later.</h2>
    <p class="title-zh">先体验场景，再了解知识。</p>
    <div class="grid-3">
      <div class="card amber"><div class="label">Story emails</div><p>The client’s tone shows pressure and stakes.</p></div>
      <div class="card blue"><div class="label">Short hints</div><p>Each control explains cost and risk in plain words.</p></div>
      <div class="card teal"><div class="label">Result cards</div><p>“This happened because of your earlier choice.”</p></div>
    </div>
  </div>
</section>

<!-- 9 AI -->
<section class="slide" id="s9">
  <div class="slide-bar"></div>
  <div class="slide-body">
    <div class="slide-num"><span>09</span> Role of AI <span class="zh">AI 扮演什么角色</span></div>
    <h2 class="slide-title">Rules stay fair. AI makes the world feel alive.</h2>
    <p class="title-zh">规则保证公平；AI 让情景更生动</p>
    <div class="grid-2">
      <div class="card teal">
        <div class="label">Rules engine</div>
        <div class="value">Scores &amp; hard limits</div>
        <p>Same inputs → same outcomes. Fair for grading.</p>
      </div>
      <div class="card blue">
        <div class="label">Large language models (optional)</div>
        <div class="value">Emails, samples, replies</div>
        <p>More natural pressure and variety—without giving “the answer.”</p>
      </div>
    </div>
    <div class="quote">AI assists the story. Students still make the judgment.</div>
  </div>
</section>

<!-- 10 Example A -->
<section class="slide" id="s10">
  <div class="slide-bar coral"></div>
  <div class="slide-body">
    <div class="slide-num"><span>10</span> Challenge A <span class="zh">挑战示例 A</span></div>
    <h2 class="slide-title">How much machine translation will you use?</h2>
    <p class="title-zh">你会用多少机器翻译？</p>
    <div class="grid-3">
      <div class="card teal">
        <div class="label">Use little</div>
        <div class="value">Safer quality</div>
        <p>But almost no spare time later.</p>
      </div>
      <div class="card coral">
        <div class="label">Use a lot</div>
        <div class="value">Cheaper &amp; faster</div>
        <p>Client may complain hard next round.</p>
      </div>
      <div class="card amber">
        <div class="label">Skip the term list</div>
        <div class="value">Save a little money</div>
        <p>Creates chaos when the team reuses text later.</p>
      </div>
    </div>
  </div>
</section>

<!-- 11 Example B -->
<section class="slide" id="s11">
  <div class="slide-bar amber"></div>
  <div class="slide-body">
    <div class="slide-num"><span>11</span> Challenge B <span class="zh">挑战示例 B</span></div>
    <h2 class="slide-title">Three problems arrive on the same day</h2>
    <p class="title-zh">三件事同一天砸过来</p>
    <div class="grid-3">
      <div class="card coral">
        <div class="label">People</div>
        <div class="value">Lead translator is ill</div>
        <p>Unfinished work. Deadline cannot move.</p>
      </div>
      <div class="card amber">
        <div class="label">Change</div>
        <div class="value">Client adds more text</div>
        <p>No extra money. No extra days.</p>
      </div>
      <div class="card blue">
        <div class="label">Legal</div>
        <div class="value">Copyright risk</div>
        <p>Their company may share the blame.</p>
      </div>
    </div>
    <div class="quote">Early planning becomes the toolkit they need today.</div>
  </div>
</section>

<!-- 12 Assessment -->
<section class="slide" id="s12">
  <div class="slide-bar teal"></div>
  <div class="slide-body">
    <div class="slide-num"><span>12</span> Assessment <span class="zh">如何评估</span></div>
    <h2 class="slide-title">We grade the thinking, not one “best path”</h2>
    <p class="title-zh">评的是思考过程，不是唯一标准答案</p>
    <div class="grid-2">
      <div class="card blue">
        <div class="label">What we collect</div>
        <ul class="clean">
          <li>Each round’s decisions</li>
          <li>How budget / quality / trust moved</li>
          <li>A short reflection at the end</li>
        </ul>
      </div>
      <div class="card teal">
        <div class="label">What “good” looks like</div>
        <ul class="clean">
          <li>Can explain why they chose this</li>
          <li>Can link today’s pain to an earlier choice</li>
          <li>Uses AI as a helper, not a blind autopilot</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<!-- 13 Close -->
<section class="slide hero" id="s13">
  <div class="slide-body">
    <div class="eyebrow">
      Takeaway
      <span class="zh">总结</span>
    </div>
    <h1>Cause and effect is the gameplay</h1>
    <p class="title-zh">决策的因果关系，就是核心玩法</p>
    <p class="close-line">Rules keep outcomes fair and repeatable. AI can make the story more vivid. Judgment stays with the students.</p>
    <div class="hero-meta" style="margin-top:1.25rem">
      <span class="chip solid">Thank you</span>
      <span class="chip">Questions &amp; playtest welcome</span>
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
