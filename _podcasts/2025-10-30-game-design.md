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
  <video controls preload="metadata" style="width: 100%; border: 1px solid #eee; border-radius: 10px; background: #000;">
    <source src="https://pub-f74b9fb442714a7b82a0ca9fd7337260.r2.dev/chezvivian_github/%E6%B8%B8%E6%88%8F%E8%AE%BE%E8%AE%A11-4%E7%AB%A0.mp4" type="video/mp4">
    你的浏览器暂不支持 HTML5 视频，请使用备用链接：
    <a href="https://pub-f74b9fb442714a7b82a0ca9fd7337260.r2.dev/chezvivian_github/%E6%B8%B8%E6%88%8F%E8%AE%BE%E8%AE%A11-4%E7%AB%A0.mp4" target="_blank" rel="noopener">直接播放视频</a>
  </video>
  <div style="font-size: 0.9rem; color: #666; margin-top: 6px;">如需在新窗口观看，请点击：
    <a href="https://pub-f74b9fb442714a7b82a0ca9fd7337260.r2.dev/chezvivian_github/%E6%B8%B8%E6%88%8F%E8%AE%BE%E8%AE%A11-4%E7%AB%A0.mp4" target="_blank" rel="noopener">在 Cloudflare R2 中播放</a>
  </div>
</div>

## Game jargons 游戏行话

<div style="margin-bottom:2em; border:1.5px solid #bbb; border-radius:12px; background:#fff; padding:24px 18px; max-width:1000px;">
  <h2 style="margin-top:0;">术语词汇表</h2>
  <ul style="list-style:none; padding:0; margin-top:1em;">
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">007时刻 (007 Moments)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        提升体验的元素。一种当你发现时能给你某种特别的夸夸反馈、动画画面和得分的游戏元素。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">决定性测试 (Acid Test)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        一种让我们在执行创意之前先测试这个创意的方法。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">肾上腺素注射场景 (Adrenalizer Scene)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        加点刺激元素以防节奏变慢的场景。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">3A游戏 (AAA Game)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        业界对顶级游戏的称呼。可以将其分解为A级艺术设定（图像和故事）、A级玩法设定以及A级程序。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">能力增长 (Ability Progression)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        游戏中的系统在玩家完成了特定任务后让其掌握新的招式、获得新的角色特性或者提升角色性能。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">阵营九宫格 (Alignment Chart)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        所有的角色将被安排到一个3×3的九宫格阵营表中，分别对应善良、中立、邪恶，以及守序、中立和混乱这两组特质的组合。出自《龙与地下城》。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">青铜、白银、黄金 (Alpha, Beta, Gold)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        游戏制作的三个主要的里程碑。青铜阶段：游戏已经基本组装完毕，但是设定、玩法和关卡仍然在调整之中。白银阶段：游戏已经完成，现在的任务是进行测试。黄金阶段：游戏完成。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">寻找弹药 (Ammo Hunt)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        一种特殊的游戏过程的简称，即搜索游戏道具和能力提升的过程。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">刺激剂 (Amphetamize)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        肾上腺素注射场景的结构形式，也就是在故事中刻意增加紧迫性。比方说倒计时就是一种刺激剂。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">动态分镜 (Animatic)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        一种简单的动画分镜，根据需要加入对白、音乐和音效，旨在让人明白最终产品的节奏是什么样的。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">街机小游戏 (Arcader)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        在一个大型的非街机游戏中引入的街机风格小游戏。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">臀部镜头 (Ass Cam)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        从身后视角跟踪的镜头（一般是身后低视角）。这是第三人称动作游戏的标准视角，比如《古墓丽影》。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">夸夸反馈 (Attaboys)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        玩家完成了某事之后出现的小型庆贺元素。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">声音游戏 (Auricular Gameplay)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        基于声音进行的游戏玩法。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">顶视 (Axonometric)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        游戏中所有的视角都是顶视视角，场景都是平面2D的场景。参考等距视角。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">意外收获 (Backhook)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        玩家在游戏前期进行的选择给后续关卡所带来的出乎意料的报偿。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">宋兵乙 (Barneys)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        可以随意消耗的游戏角色。来自《半条命》中各种保安的人物模型。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">故事节拍 (Beats)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        故事节拍是单独的情节元素，它们组合起来构成一个大的故事。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">唐僧 (Bitching Bettys)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        在游戏过程中冒出来的角色，用来推动或者引导玩家去完成一些特定的动作，同样可以用作警告装置。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">强推 (Blowpast)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        游戏中能够让玩家强行通过一个他无法完成的关卡或者挑战的机制，这样他就不会卡在游戏的某个关卡中。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">蓝鞋子 (Blue Shoes)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        如果你在为一个客户做项目，你交付的内容必须是合乎他们想法的版本，就算你觉得自己有个更好的想法也不行。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">换皮 (Blueprint Copying)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        &quot;让我们来&#x27;抄袭&#x27;一下这个游戏，但是我们得换掉这个科幻冒险的皮，把它做成西部风格&quot;这种创意过程。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">邦德视角 (Bond Sense)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        玩家可以通过这个模式进入一个有别于角色的视角。该视角将为玩家提供必要的信息或者有趣的任务。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">拉皮效应 (Botox Effect)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        真实演员和逼真的角色之间仍然存在的差异。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">游戏分支 (Branch)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        游戏中脱离故事主线（最佳路径）的部分。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">多分支结构 (Branching)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        交互式冒险游戏中的术语。在这个结构中，故事会根据玩家的选择导向不同的结局或者情节发展。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">破坏游戏 (Breaking the Game)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        玩家在游戏的设计、AI或代码中寻找到弱点，让他们能够用一种非预期的方式胜利。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">按钮捣碎机 (Button Masher)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        你在这种游戏里不需要学习招式技巧，只需要随便按键就能通关。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">指令 (Call-Outs)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        给玩家提供方向的对白。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">假幽默 (Camedy)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        假装幽默。指书中所有角色都被某些看似搞笑，实则只是为了表现这件事有趣的东西给逗乐了。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">镜头逻辑 (Camera Logic)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        镜头背后的动机。杀手的视角、旁观者的视角、老师的视角等镜头的顺序就构成了叙事。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">计算机生成图像 (CGI)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        computer-generated imagery的缩写。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">角色冒险 (Character Adventure)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        玩家控制一个特定的、标志性的角色进行冒险的游戏类型。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">作弊码 (Cheats)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        玩家输入就可以赢得游戏、获得道具或者升级的代码。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">&quot;听上去不错&quot;型决策 (CIG)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        &quot;听上去不错&quot;即&quot;开会的时候听上去不错&quot;。它指的是那些讨论的时候感觉不错，但实际上要么没有意义，要么所有人都很喜欢但却根本实现不了的情况。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">过场动画 (Cinematic)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        游戏的叙事段落。一般情况下玩家会失去部分操作性。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">清洗 (Cleansing)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        必须浏览一遍剧本或者文档，清洗掉所有的创意痕迹（一般为了清权）。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">克林贡人 (Clingons)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        指某些死抱着某个项目，但是没有权利这么做的人。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">小丑车 (Clown Car)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        在游戏里用来不停给主角练手（电影里也会有）。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">收集品 (Collectable)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        玩家在游戏过程中可以捡起来用的物品和对象，比方说弹药、血包、增强剂等。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">连招 (Combos)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        一系列可以完成更加强大的攻击的招式。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">完成度 (Completion Rate)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        衡量玩家完成游戏的程度。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">设定 (Conceit)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        游戏里需要玩家发自内心接受的想法。比方说，一个游戏的设定可能是总在下雨。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">概念文档 (Concept Document)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        一个阐述了游戏的基本机制、设定、样式、情感、情节、世界观等元素的简短文档（大概10页）。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">条件目标 (Conditional Objective)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        为了做X事件，你得先完成Y事件。例如为了开一扇门，你得先找到门卡。参考&quot;锁-钥匙&quot;机制。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">后果 (Consequences)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        玩家之前所做出的决定会在之后的故事中影响到他。这也表明游戏世界是有记忆的。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">合作模式 (Co-Op)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        多人游戏中，玩家组成一队对抗电脑，也称合作模式。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">关键路径 (Critical Path)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        一个多分支结构游戏里的主要故事或游戏路径，同样适用于游戏开发中描述项目完成所必须执行的主要路径。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">剧情画面 (Cut-Scene)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        与过场动画类似，但是更多情况下使用引擎实时渲染，也被称为&quot;游戏内动画&quot;。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">&quot;死亡情节&quot;替代元素 (Death Equivalents)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        在面向儿童的项目中，会加入一些元素避免展现死亡场景。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">交付作品 (Deliverables)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        项目开发时必须交付的实际工作。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">破坏蝙蝠车 (Denting the Batmobile)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        胡搞神圣的东西。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">设计文档 (Design Document)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        游戏开发的蓝图。开发过程中会有很多的修改和迭代工作。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">可破坏场景 (Destructible Environment)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        在关卡内可以破坏的场景。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">开发商 (Developers)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        实际制作游戏的公司或团队。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">钻石分支 (Diamond Branching)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        游戏中的一个短分支，进入之后会很快回到主线，是一种数量非常有限的分支类型。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">有引导的体验 (Directed Experience)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        玩家拥有控制权，但是整个游戏采用的是一个在已经确定好的情况下给予玩家丰富游戏体验的线性设计。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">设计师的无用想法 (DWUK)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        Design Wanker&#x27;s Useless Concern的简称。设计师顾虑了太多没有实际意义的事情。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">动态音乐 (Dynamic Music)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        音乐随着环境或者情况的变化而变化，没有固定顺序。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">电梯推销 (Elevator Pitch)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        一种你可以在电梯里与一位总裁或者制作人说完的非常简短的推销方式。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">自发玩法 (Emergent Gameplay)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        事情并不总是按照设计师的构思来发生。有些时候玩家会找到一个很有趣但你从来没想过的办法来折腾游戏。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">引擎 (Engine)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        所有游戏都有的代码结构。引擎有很多分类，比方说物理引擎和图形引擎。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">事件触发 (Event Trigger)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        一个动作、地点或者对象触发了一些新的事件，让游戏剧情继续前进。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">展示 (Exposition)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        用来构建故事、世界和角色的信息。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">衍生价值 (Extrinsic Value)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        在游戏之外用来提高游戏体验的东西，包括网页、漫画、营销活动等。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">眼睛糖果 (Eye Candy)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        漂亮的图像和美术。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">虚假宣传 (Faux Pitch)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        在宣传中听着很不错，但是实际上会因为各种各样的原因没有办法实现的点子。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">恐惧对象 (Fear Object)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        在故事中指角色害怕的事物。在项目开发中，它是你在项目中害怕的事物。参考&quot;保护创意&quot;。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">特性蔓延 (Feature Creep)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        在游戏开发过程中额外加入的玩法元素。这个词绝大多数情况下用在贬义语境，用来表明团队和设计失去了重点。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">反馈循环 (Feedback Loop)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        你按下一个键，一些有意义的事情发生了。你理解了发生的事情。重复这个过程。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">跑腿任务 (Fetch Quest)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        让你去跑腿拿东西的任务。这是最基本的游戏设计元素，而且很乏味。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">第一人称视角 (First-Person POV)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        游戏以角色的视角来展现，就像通过他们的眼睛观察周围环境，为玩家创造一种他和游戏角色是同一人的感觉。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">心流状态 (Flow State)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        你达到某种状态时就不会注意到时间的流逝，同样称为&quot;心流区域&quot;。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">冲走 (Flushed)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        没了。从设计里删掉了，游戏里没有了。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">全动视频 (FMV)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        Full-Motion Video的简称。指交互式真人视频。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">某某 (Foo)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        创作人员所不需要了解的技术术语。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">原力 (Force)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        让玩家按特定的方向走或者进行特定的动作，然而又维持玩家自由选择的幻觉的某种魔法和艺术。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">分位重写 (Fractile Rewrite)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        系统性地过一遍剧本，搜索某个特定的元素——比方说一个角色，然后重写。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">冻结 (Freeze)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        即停止修改，可用于代码、美术、设计、特性。一个游戏到了代码冻结状态，游戏引擎就不再增加或者删除元素了。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">乐趣元素 (Fun factor)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        &quot;没错，这个设计想法很酷。但是玩家真的会觉得这有趣吗？乐趣元素是什么？&quot;等相当普遍的问题。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">游戏逻辑 (Game Logic)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        游戏逻辑决定了游戏中所有的功能必须都是有意义的。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">游戏目标 (Game Objective)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        手上的任务，玩家要做的事情。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">玩家骄傲 (Gamer Pride)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        在游戏设计中增强玩家能力的行为。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">苏门答腊巨鼠 (Giant Rat of Sumatra)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        一个系列作品中让人好奇、悬而未决的故事。这个术语是致敬《福尔摩斯》系列。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">下水 (Gibs)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        角色被击中的时候飞起来的身体部分。家禽下水（Giblets）意译而来。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">格拉沃奇 (Glavotch)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        过分复杂的发明。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">老古董 (Gornished)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        过时了但并不完全是一堆垃圾的东西，大家就是不喜欢或产生了审美疲劳。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">颗粒 (Granular)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        用最小的细节来解释更重要的问题。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">老兵 (Grognard)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        战争游戏玩家。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">意会 (Grok)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        你如此清楚地理解某件事情，甚至都不用去思考。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">接地气 (Grounding)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        将游戏设定得容易理解。比方说设定游戏发生在一个熟悉的世界，里面都是熟悉的角色，也是熟悉的游戏类型。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">清版 (Hack and Slash)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        打穿一波接一波的敌人。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">叠床架屋 (Hat on a Hat)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        一个概念里塞了太多点子。一个角色戴着牛仔帽可以让他看着像个牛仔，但是牛仔帽上再戴着棒球帽，那他的样子看上去就有点不太聪明。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">转头 (Head Turn)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        角色在场景里转头去看某个可能有意义的对象，也是另一种用来让玩家知道要去注意某个东西的办法。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">平台动作 (Platformer)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        要求玩家从一个平台跳到另一个平台的游戏（《狡狐大冒险》《古惑狼》）。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">热点 (Hot Spot)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        指玩家或者指针移动到某个会触发特定动作的特定区域。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">创意稀释 (Idea Diffusion)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        基本创意在开发后被弱化。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">创意漂移 (Idea Drift)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        失去了设计和故事，或者二者之一的核心元素，加入了太多的点子。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">自由幻觉 (Illusion of Freedom)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        优秀的沙盒游戏会试图给你这种印象。这个世界总是一个幻觉，限制和拘束总是存在的。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">不可避免的游戏 (Inevitable Game)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        游戏一定会被制作出来，一旦最初的兴奋消退，时间表和预算的现实就登场了。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">即刻乐趣 (Instant Fun)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        拿起手柄、开始玩带来的乐趣。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">界面 (Interface)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        图形游戏的惯例，向玩家提供信息，帮助他与游戏互动。例如血条、弹药计数器、地图等。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">物品栏 (Inventory)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        角色携带的物品。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">隐形曲线 (Invisible Ramp)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        玩家继续玩下去，游戏变得越来越有挑战性。这是设计基本原则之一。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">等距视角 (Isometric Camera)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        从上向下斜视45度，更加有纵深感的视角。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">这是个特性！ (It&#x27;s a Feature!)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        一种欢乐的事故，指游戏里一开始是漏洞或者错误的东西最终变成了一种全新的玩法。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">主意很酷但不好玩的点子 (K.I.N.F)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        Kool Idea, No Fun的简称。这种点子在概念上很坚实，但是无法构造出有趣的玩法。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">主意很酷但实现不了的点子 (K.I.N.I)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        Kool Idea, Not Implementable的简称。想法很好，但是不切实际。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">保持简单，蠢货 (K.I.S.S)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        Keep It Simple, Stupid的简称。老话了，但是仍然值得记住。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">别断气 (Keeping Alive)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        提醒玩家某个角色在游戏的某一部分里并没有什么用处，同样用于保留若干情节元素。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">杀掉恺撒 (Killing Keyser)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        这是一种非常有破坏力的文档，如果你不搞定它，整个项目都会崩溃。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">有道理但没意思的想法 (L.I.N.F)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        Logical Idea, No Fun的简称。意思同该术语的名字。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">铺设管子 (Laying Pipe)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        去做某些之后会带来报偿的事情。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">学习曲线 (Learning Curve)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        宏观的学习曲线指玩家玩游戏时学习技巧和概念的过程。微观的学习曲线指如何在任务中击败特定的角色。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">关卡 (Levels)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        即游戏的场景。游戏里的关卡就像书中的章节。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">外观和感受 (Look and Feel)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        外观是指游戏的画面，感受是指玩游戏的感觉。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">&quot;路易吉&quot;关卡 (Luigi)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        安抚玩家的模拟练习。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">招牌 (Marquee)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        你的卖点是什么——有名的IP、经典作品的续作还是著名的设计师？
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">机制 (Mechanic)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        游戏里与玩家互动的核心玩法。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">元故事 (Metastory)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        互动项目的元故事指故事中所有角色的故事或者隐藏背景的集合，包括所有的分支和对白、可能的结局以及背景故事，即整个游戏世界。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">中间件 (Middleware)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        授权用来开发游戏的游戏引擎。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">里程碑 (Milestone)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        项目前进所必须达到的关键节点。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">基于任务的玩法 (Mission-Based Gameplay)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        玩家需要完成一系列指定任务来通过一个关卡。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">单调 (Monotonatic)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        同样的颜色，同样的音乐，同样的游戏机制。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">&quot;钓&quot;鼠标 (Mouse Fishing)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        指老式的CD-ROM游戏，你得到处移动鼠标，直到撞上什么有趣的东西触发。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">胡子 (Moustache)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        伪装新元素，将其与熟悉的旧有版本分开。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">现在我们来研究一下真游戏到底是什么 (Now We&#x27;ll Figure Out What the Real Game Is)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        开发过程中的一个非正式的流程，通常会发生在人们意识到资金、美术、容量、编程时间都有限制的时候。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">非玩家角色 (NPC)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        Nonplayer Character的简称。玩家不能控制的角色都是非玩家角色。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">范式破坏者 (Paradigm Buster)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        一个游戏或者电影惊为天人，乃至从根本上改变了这个媒介，变成了一个新的类型。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">平行设计过程 (Parallel Design Process)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        同时处理一个项目中的3个主要元素，并立即衡量一个领域在另一个领域的突破。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">巴甫洛夫 (Pavlovian)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        有个说法是，游戏设计都是巴甫洛夫式的。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">报偿 (Payoffs)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        奖励玩家的任何事情。在故事层面，指设定的叙事结果。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">搞砸 (Pear-Shaped)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        在以任务为基础的游戏中，由于描述剧本或随机事件出错导致玩家需要自由发挥的情况。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">王小明 (Pete Popcorn)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        你的受众的一般形象。这里的要点在于你必须将自己的受众还原成一个具体的人，虽然这个还原可能很粗略。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">爆米花反应 (Popcorning)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        一个东西爆炸了，它旁边的东西跟着爆炸了，进而产生了一系列连锁反应来消灭敌人。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">初步设计文档 (Preliminary Design Document)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        这是一份包含更多游戏细节的比较长的文档（大概有50到200页）。理想情况下，文档中还应该包括一些美术细节。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">保护创意 (Protecting an Idea)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        &quot;你保护的是什么？&quot;是经常发生的争论，因为某人会想要留着项目里的某个元素。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">原型 (Prototype)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        游戏开发中一个可以玩的模型，用来测试核心玩法概念是否行得通，以及游戏能否在时间和预算允许的情况下做出来。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">游戏厂商 (Publishers)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        制作、宣传并销售游戏的公司，大多数时候也给游戏开发提供版权。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">快速理解特性 (QRFs)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        Quickly Recognized Features的简称。玩家拿到一个游戏后能够马上上手，因为这个类型的游戏的操控方法与其他游戏是类似的。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">布娃娃 (Ragdoll)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        真实的物理机制。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">红衫 (Red Shirt)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        注定会死的角色，出自《星际迷航》。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">参考作品 (Reference Titles)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        你应该知道的某个用来理解一个特定设计的作品。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">重新载入学习 (Reload Learning)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        指反复尝试某个关卡来学习操作方法的过程。基本上，你玩的次数越多，就能理解得越好。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">重玩性 (Replayability)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        所有线性故事的游戏（包含一个结尾）都注定在可重玩性上有限制。你体验完了故事，游戏就结束了。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">混剪 (Ripamatics)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        从广告行业&quot;偷来&quot;的术语，指使用现有的视频或者其他电影、电视剧里的片段拼起来的概念视频。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">墨迹测试 (Rorschach)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        指一份可以设计出来让读者或评委看到他们想看到的内容的文档或者范例。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">压盘制作 (RTM)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        Release to Manufacture的简称。你的完成版在这个阶段脱离了你的掌握，进入压盘的流程。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">沙盒 (Sandbox)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        游戏中玩家可以自由行动，做随机任务，并不局限于故事线的区域。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">日程表猴子 (Schedule Monkey)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        每个开发商都会有的那个家伙，他会告诉你不能这样做，因为日程表不允许。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">很复杂的麻烦 (Schlobongle)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        词意如其名。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">剧本论述 (Scriptment)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        介于剧本和故事阐述之间，包括整个故事、对白片段、场景、镜头视角等。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">掌控感 (Sense of Mastery)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        玩家玩游戏时产生的那种觉得自己掌握了游戏和整个世界的感觉。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">巧合因素 (Serendipity Factors)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        游戏中没有预料到却变成了最终目标的元素。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">约定俗成的事情 (SFAR)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        Standard for a Reason的简称。指游戏玩法中的一些规则在业内是约定俗成的事情，玩家凭借直觉便可完成。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">音效 (SFX)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        Sound Effects的简称。游戏中的各种声音。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">小点子 (Snags)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        某些你想要从其他游戏里扒出来，塞进自己的游戏里的设计元素。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">打野 (Snipe Hunting)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        让玩家在游戏里无止境地漫游，去寻找某些游戏里不存在或者被隐藏起来的东西。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">给屎打光 (Spotlight on a Turd)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        过度强调某个情节或者游戏的问题，吸引玩家不必要的注意力。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">进度条时长 (Start to Crate Ratio)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        你从开始游戏到遇到第一个游戏套路之间所花的时间。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">隐蔽教育 (Stealth Education)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        一种通过沉浸式玩法达到教学目的的游戏机制。玩家会知道他们到底有没有学到技能。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">故事板 (Storyboard)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        在正式制作之前，艺术家画出来让动作可视化的草稿。它同样可以用来让大家大致理解玩法。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">初始人物或空白模板 (Tabula Rasa)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        玩家从零开始创建角色或整个世界，赋予其独特的身份。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">技术设计文档 (Technical Design Document)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        游戏设计文档的补充，专注于开发过程中程序和代码层面的问题。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">泰施坦因定律 (Tezstein&#x27;s Law)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        你处理掉了一个没有能力或者很烦人的经理人，那么代替他的人选必然比他更烂。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">三只手 (Third-Handed)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        用来描述非常复杂的游戏玩法，你需要三只手才能很好地进行操作。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">第三人称视角 (Third-Person Point of View)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        玩家可以看到游戏的主要角色的视角。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">这不是我的第一次野餐 (This Is Not My First Picnic)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        你之前做过，能理解这其中蕴含的问题和危险。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">手指糖果 (Thumb Candy)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        优秀的玩法。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">倒计时 (Ticking Clock)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        给玩家设定一个有限的时间，增加紧张感。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">作品 (Title)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        游戏本身。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">信息过量 (TMI)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        Too Much Information的简称。玩家实际需要知道哪些信息才能理解游戏规则和故事？
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">可玩具化 (Toyatic)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        这个系列能不能出玩具？具不具有玩具化的潜力？
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">战壕大衣 (Trench Coat)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        用来掩盖那些不好看的东西的伪装物。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">系列设定 (Trivbits)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        游戏中所插入的与游戏可能没有关联但却塑造了整个游戏系列的元素。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">主体 (Trunk)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        在一个有限分支游戏中，故事的主线、优先路径以及分支在主体处交会。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">调试修改 (Tune and Tweak)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        优化玩法和关卡细节。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">萝卜车赌博 (Turnip Truck Gambit)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        有些人会给你提供一个条件很烂的交易，觉得你根本不知道自己在做什么。这经常是侮辱性的。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">忍者神龟化 (Turtling the Ninja)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        将某些人不能接受的概念&quot;软化&quot;或变形使其接受。这来自20世纪80年代的《忍者神龟》系列。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">独特卖点 (USP)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        Unique Selling Points的简称。游戏中能够吸引玩家买游戏的那些元素和特质。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">价值系统 (Value System)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        游戏的&quot;世界&quot;里的价值是什么？这个世界的&quot;道德&quot;是什么？
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">方向检查 (Vector Check)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        检查项目的时候问一下自己&quot;这是不是我想要去的方向&quot;。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">垂直切片 (Vertical Slice)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        游戏演示中的一个特别类型。整个预期游戏中的一小部分被从头到尾做完，有完整的设计、游戏机制、美术效果以及运行程序。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">&quot;暴力情节&quot;替代元素 (Violence Equivalents)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        在儿童游戏里很常见，比方说用玩具枪取代真枪（射出凝胶）。用来软化暴力的手段。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">愿景 (Vision)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        无形的、可以共享的、推动项目前进的观点。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">5W1H (5W1H)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        游戏故事结构的基本要素，即谁（Who）、什么（What）、何时（When）、何地（Where）、为何（Why）、怎样（How）。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">攻略 (Walkthrough)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        对指定关卡的游戏体验的文字描述。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">路点 (Waypoints)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        关卡中的关键位置。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">铲除杂草 (Weed Eating)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        从设计和故事中处理掉不必要元素的过程。
      </div>
    </li>
    <li style="margin-bottom:14px;">
      <div style="font-weight:bold;">人海战术 (Zerging)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        没有技巧的玩法，更依赖于数量而非战略（名字来自《星际争霸》中的某个外星人种族）。
      </div>
    </li>
  </ul>
</div>
