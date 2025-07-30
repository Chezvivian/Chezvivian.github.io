---
layout: single
title: "许家金：大语言模型辅助外语教学"
---

<div style="margin-bottom: 2em;">
  <a href="/podcasts/2025-07-29-English-teaching" style="color: #007acc; text-decoration: none; font-weight: 500;">← 返回"大语言模型辅助商务英语教学"播客主页</a>
</div>

* TOC
{:toc}

## 基本信息

资料来源：许家金, 赵冲, 孙铭辰. 大语言模型的外语教学与研究应用[M]. 外语教学与研究出版社, 2024.

书籍配套网页：[https://corpus.bfsu.edu.cn/info/1082/1914.htm](https://corpus.bfsu.edu.cn/info/1082/1914.htm)

许老师整理的大模型资源链接：[大模型链接大全](https://corpus.bfsu.edu.cn/CorporaAZ.htm)

许老师整理的大模型提示库网站：[提示语集合](https://promptbank.unipus.cn)

**如果没有时间阅读这个长文档，你也可以听一听这个音频，是把这个网页凝练总结的两个主持人对话（用 NotebookLM 生成）。听一听试试！**

<audio controls style="width: 100%; max-width: 600px; margin: 2em 0;">
  <source src="/files/podcasts/English-teaching/大语言模型辅助商务英语教学研究.wav" type="audio/wav">
  您的浏览器不支持音频播放。
</audio>

**以下是从内容中提取出来，你可能会感兴趣的术语表。**

<div style="margin-bottom:2em; border:1.5px solid #bbb; border-radius:12px; background:#fff; padding:24px 18px; max-width:1000px;">
  <h2 style="margin-top:0;">关键术语词汇表</h2>
  <ul style="list-style:none; padding:0; margin-top:1em;">
    <li style="margin-bottom:10px;">
      <div style="font-weight:bold;">大语言模型 (LLM)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        能够理解和生成人类语言的人工智能模型，具有处理、理解和生成文本的能力，可用于多种语言教学任务。
      </div>
    </li>
    <li style="margin-bottom:10px;">
      <div style="font-weight:bold;">产出导向法 (Output-driven Approach)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        一种外语教学理论，强调以学习者的语言产出为导向，通过“驱动”、“促成”、“评价”等环节，促进语言习得。
      </div>
    </li>
    <li style="margin-bottom:10px;">
      <div style="font-weight:bold;">续论 (Continuation Theory)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        一种语言习得观，强调通过“续写”、“续说”、“续译”等形式，将语言理解（输入）和语言产出（输出）紧密结合，在动态过程中实现语言习得。
      </div>
    </li>
    <li style="margin-bottom:10px;">
      <div style="font-weight:bold;">CEFR (Common European Framework of Reference for Languages)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        欧洲共同语言参考标准，用于描述语言能力水平的国际标准，如A1、A2、B1、B2、C1、C2。
      </div>
    </li>
    <li style="margin-bottom:10px;">
      <div style="font-weight:bold;">词根构词法 (Root-based Word Formation)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        通过理解词根（如“port”）来推导和记忆相关单词（如“transport”、“import”）含义的方法。
      </div>
    </li>
    <li style="margin-bottom:10px;">
      <div style="font-weight:bold;">近义词辨析 (Synonym Discrimination)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        区分意义相近但用法、语境或细微差别不同的词汇（如“fare”和“fee”）。
      </div>
    </li>
    <li style="margin-bottom:10px;">
      <div style="font-weight:bold;">熟词生义 (New Meanings of Familiar Words)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        指常见词汇或短语在特定语境下产生新的或引申的含义（如“get around”）。
      </div>
    </li>
    <li style="margin-bottom:10px;">
      <div style="font-weight:bold;">部分倒装句 (Partial Inversion)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        英语语法中一种特殊的句式结构，当否定副词（如“never”、“hardly”）置于句首时，句子的部分谓语会提前到主语之前。
      </div>
    </li>
    <li style="margin-bottom:10px;">
      <div style="font-weight:bold;">宾语补语 (Object Complement)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        用于补充说明宾语的成分，可以是形容词、名词、现在分词、不定式等。
      </div>
    </li>
    <li style="margin-bottom:10px;">
      <div style="font-weight:bold;">人工智能后编辑 (AI Post-editing)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        指对大语言模型生成的内容进行人工审核、修改和调整，以确保其准确性、符合教学要求和语言自然度。  
      </div>
    </li>
    <li style="margin-bottom:10px;">
      <div style="font-weight:bold;">音节接龙 (Syllable Chain Game)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        一种口语活动，通过音节划分帮助学生掌握多音节单词的发音和拼写，通常是前一个词的尾音节是后一个词的首音节。
      </div>
    </li>
    <li style="margin-bottom:10px;">
      <div style="font-weight:bold;">视后续说 (Visual-based Continuation Speaking)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        基于图片、视频等视觉输入，引导学生进行故事续说或内容扩展的口语练习。
      </div>
    </li>
    <li style="margin-bottom:10px;">
      <div style="font-weight:bold;">语域 (Register)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        指语言在特定交际情境（如正式、非正式、专业等）下所呈现出的词汇、语法和风格特征。
      </div>
    </li>
    <li style="margin-bottom:10px;">
      <div style="font-weight:bold;">同义改写 (Paraphrasing)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        在保持原意不变的前提下，使用不同的词汇、短语或句式对文本进行重新表达。
      </div>
    </li>
    <li style="margin-bottom:10px;">
      <div style="font-weight:bold;">交互阅读游戏 (Interactive Reading Game)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        利用大语言模型创建的、读者可以通过选择或输入来影响故事走向的阅读体验。
      </div>
    </li>
    <li style="margin-bottom:10px;">
      <div style="font-weight:bold;">思维导图 (Mind Map)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        一种可视化的工具，用于整理和呈现信息，通过中心主题和分支结构来显示概念之间的关系。
      </div>
    </li>
    <li style="margin-bottom:10px;">
      <div style="font-weight:bold;">词云图 (Word Cloud)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        通过不同大小和颜色的文字，直观地展示文本中词汇的频率和重要性。
      </div>
    </li>
    <li style="margin-bottom:10px;">
      <div style="font-weight:bold;">作文自动评阅 (Automated Essay Scoring)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        利用人工智能技术对学生作文进行多维度（如结构、语法、词汇、内容等）评估和反馈。
      </div>
    </li>
    <li style="margin-bottom:10px;">
      <div style="font-weight:bold;">提示语 (Prompt)</div>
      <div style="margin-top:6px; color:#444; background:#f8f8f8; border-radius:6px; padding:8px 12px;">
        向大语言模型发出的指令或问题，用于引导模型生成特定内容的文本。
      </div>
    </li>
  </ul>
</div>


## Part I. 词汇篇

### 1. 词根构词拓展学习

- 通过词根理解词义并拓展词汇
  - **词根构词拓展练习**：基于特定词根（如port）设计选择题，引导学生通过词根关联记忆相关单词。学习包含相同词根的单词群（如transport、import、export、report等），理解词根的基本含义。

```
Please create [number] multiple-choice questions each focusing on a different word derived from the root "[词根]". For each question:
1. 指定任务：提供词汇释义题目，选项为含有相同词根的词汇
2. 目标群体：未明确指定，可根据难度调整
3. 举例：未在提示中提供
4. 具体要求：为每个问题提供正确答案
```

### 2. 围绕特定主题造句成段

- 产出导向法中的语言促成设计
  - **特定主题造句成段练习**：围绕中心意义组句成段，教师引导学生选定特定关联词汇进行造句成段练习。建立以功能为中心的目标语言意义关联，带动多个目标词汇的学习和产出。

```
Please generate [number] interconnected words that are suitable for CEFR [级别] level learners and can be used in the context of "[主题]". 
1. 指定任务：生成相互关联的词汇并设计段落写作任务
2. 目标群体：明确指定语言水平（如CEFR B1级别的学习者）
3. 举例：提供示例段落，展示如何使用目标词汇
4. 具体要求：词汇应涵盖特定主题的不同方面，并用于写作任务
```

### 3. 指定英语词汇的读后续写材料设计

- 基于"续论"语言习得观的读后续写练习  
  - **读后续写练习**：提供含有指定教学词汇的阅读材料，引导学习者在充分理解语篇的基础上续写内容。将语言产出与语言理解紧密关联，通过"续"习得语言。输入方式为阅读，输出方式为写作。

```
Please create a reading-writing integrated continuation task suitable for CEFR [级别] level learners about "[主题]". The reading passage should be approximately [字数] words long and incorporate the following [number] words: "[词汇1]", "[词汇2]", etc.
1. 指定任务：创建读后续写练习，包含阅读材料和写作任务
2. 目标群体：明确指定语言水平（如CEFR B2级别）
3. 举例：提供阅读材料和续写任务示例
4. 具体要求：阅读材料长度、难度和必须包含的目标词汇
```

### 4. 近义词词义辨析（fare和fee）

- 帮助学生辨析近义词的意义差异
  - **近义词选词填空练习**：设计填空题，让学生根据语境选择正确的近义词。通过语境对比分析词义差异（如fare指交通运输相关费用，fee指服务、许可证、会员资格等相关费用）。提供答案解析，概括不同词汇对应的不同语境和用途。

```
Please create [number] fill-in-the-blank questions (using "[词1]" or "[词2]") to distinguish the meanings of "[词1]" and "[词2]" and provide the answers along with explanations.
1. 指定任务：创建选词填空题，区分两个近义词的含义
2. 目标群体：未明确指定
3. 举例：未在提示中提供
4. 具体要求：提供答案和解释，明确各词的用法区别
```

### 5. 形式相似词的词义辨析（cloth、cloths、clothing和clothes）

- 形式相似、语义关联的词汇辨析  
  - **形式相似词改错练习**：针对形式相似的词汇设计改错题。辨析名词的可数/不可数用法及单复数形式的意义差别。
  
```
Please create [number] error-correction questions to distinguish the meanings of "[词1]", "[词2]", "[词3]", and "[词4]". 
1. 指定任务：创建改错题，判断形式相似词在句中是否使用正确
2. 目标群体：未明确指定
3. 举例：未在提示中提供
4. 具体要求：提供答案解析，解释每个词的正确用法
```

### 6. 近义词用法辨析（suggest和advise）

 
- 近义词在语用场景和句法结构上的差异  
  - **近义词判断练习**：针对近义词的用法区别生成判断练习。辨析不同词汇适用的语用场景（如suggest用于非正式场合，advise用于正式或官方场合）。明确句法结构差异（如suggest that sb. (should) do sth.，而advise sb. to do sth.）

  
```
Please provide [number] exercises to distinguish the difference between "[词1]" and "[词2]" when expressing [功能], with more than half of the sentences being incorrect.
1. 指定任务：创建正误判断题，区分两个近义词的用法
2. 目标群体：未明确指定
3. 举例：提供包含常见错误的例句
4. 具体要求：包含语用场景错误和语法结构错误的例句，并提供正误评注
```

### 7. 熟词生义问题（get around）

 
- 多义词或短语不同义项的辨析
  - **多义词/短语辨析选择题**：设计选择题帮助学生根据语境识别目标短语的不同意义。涵盖多义词/短语的基本义和引申义（如get around的"四处走动"、"克服困难"、"避开规则"等义项）。提供充足语境以便学生进行意义判断。
  
```
Please design multiple-choice questions to distinguish all the meaning of the phrase "[词组]". Please provide the answers along with explanations.
1. 指定任务：设计选择题区分多义词/短语的不同含义
2. 目标群体：未明确指定
3. 举例：未在提示中提供
4. 具体要求：提供不同语境下的例句，以及答案和解析
```
 
### 8. 易混词拼写练习

 
- 英语易混淆单词的拼写问题
  - **易混词拼写选择题**：针对拼写容易出错的单词设计选择题。包含常见拼写错误（如重复字母问题、字母顺序错误、额外字母添加等）。
  
```
Design a context-based multiple-choice spelling quiz for the words "[词1]", "[词2]", "[词3]", etc. 
1. 指定任务：设计基于语境的拼写选择题
2. 目标群体：明确指定语言水平（如CEFR B2级别）
3. 举例：未在提示中提供
4. 具体要求：为每个单词提供语境句子，包含一个正确拼写和三个常见错误拼写
```


## Part II. 语法篇

### 1. 关系从句练习设计

 
- 基于"续论"语言习得观的读后续写任务，将关系从句融入阅读材料
  - **读后续写关系从句练习**：设计包含多个英语关系从句的阅读材料，引导学生基于阅读内容进行续写。在阅读材料中嵌入多种类型的关系从句（限定性关系从句、非限定性关系从句等）。关系从句由which、who、that等关系代词引导，使学习者在阅读和续写过程中习得复杂句型。

  
```
Please create a reading-writing integrated continuation task suitable for CEFR [级别] level learners, focusing on [主题]. The reading passage should be approximately [字数] words long and incorporate [数量] relative clauses (please highlight these clauses).
1. 指定任务：创建包含特定数量关系从句的阅读材料和续写任务
2. 目标群体：明确指定语言水平（如CEFR B2级别）
3. 举例：在响应中提供续写示例
4. 具体要求：阅读材料长度和应包含的关系从句数量
```
 
### 2. 虚拟语气材料改编

 
- 基于"续论"语言习得观的强化读后续写任务，促进虚拟语气的习得
  - **强化读后续写虚拟语气练习**：改编原有英语故事，在阅读材料中融入多种虚拟语气表达。包含现实的虚拟（if only I had）、愿望的虚拟（I wish it were）、过去的虚拟（Had I known）和命令的虚拟（It's essential that...）等多种形式。通过阅读材料中明确提示相应的语法结构，增强协同效应，促进学习者对虚拟语气的习得。

  
```
Please create a reading-writing continuation task for [级别] level learner based on the story of [故事名称]. The reading segment should be around [字数] words, embedding [数量] examples of the subjunctive mood, which should be clearly marked.
1. 指定任务：改编特定故事，嵌入虚拟语气表达并设计续写任务
2. 目标群体：根据难度水平指定
3. 举例：提供原故事内容作为参考
4. 具体要求：阅读材料长度和应包含的虚拟语气例句数量
```
 
### 3. 宾语补语的用法

 
- 英语语法中宾语补语的使用和改写练习
  - **宾语补语改写练习**：设计针对不同类型宾语补语的改写练习。涵盖形容词作宾补（They considered the proposal beneficial）、现在分词作宾补（I saw her running）和不定式作宾补（I want you to stay）三大类型。

  
```
Please create a series of [数量] exercises designed for CEFR [级别] level English learners, with a focus on the use of object complements. Distribute these exercises across [数量] categories of object complements: [类型1], [类型2], and [类型3].
1. 指定任务：设计宾语补语改写练习
2. 目标群体：明确指定语言水平（如CEFR B2级别）
3. 举例：提供基础句和改写后的示例
4. 具体要求：包括不同类型的宾语补语练习和答案解析
```
 
### 4. 过去完成体和过去完成进行体的区分

 
- 英语中过去完成体和过去完成进行体的对比和应用
  - **时态填空练习**：设计针对过去完成体（had + 过去分词）和过去完成进行体（had been + 现在分词）的语法填空题。通过场景化的例句区分两种时态的用法差异（过去完成体强调动作在过去的完成，过去完成进行体强调动作在过去的持续）。结合否定句形式和副词（如already）的用法进行综合练习。

  
```
Please create [数量] grammar gap-fill questions that guide students to modify the base tense to either past perfect or past perfect continuous. Please provide the answers and explanations.
1. 指定任务：创建时态填空题，区分过去完成体和过去完成进行体
2. 目标群体：指定语言水平和主题背景（如校园生活）
3. 举例：未在提示中直接提供
4. 具体要求：为每个题目提供答案和详细解释
```
 
### 5. 否定副词引导的部分倒装句学习

 
- 英语中否定副词引导的部分倒装句结构与应用
  - **部分倒装句改写练习**：使用多种否定副词（never、rarely、seldom等）引导学生将普通句改写为部分倒装句。学习"否定副词 + be动词/助动词/情态动词 + 主语 + 谓语"的部分倒装结构。通过练习不同类型的否定副词（短语），如never、seldom、hardly、not only、in no way、at no time等，扩展学习者的语法知识。

  
```
Please create [数量] exercises on partial inversion with negative adverbials in English. For each exercise, provide the negative adverb, the original sentence, and instruct students to rewrite it as a partial inversion sentence.
1. 指定任务：设计否定副词引导的部分倒装句改写练习
2. 目标群体：通过词汇难度控制目标水平
3. 举例：为每个否定副词提供原始句和改写后的句子
4. 具体要求：使用不同的否定副词/短语创建练习并提供答案
```
 
### 6. 主谓一致问题

 
- 英语语法中主语和谓语在人称和数上的一致性规则
    - **主谓一致改错练习**：设计多种主谓一致情境的错误改正题。涵盖多种常见错误类型：单数/复数形式错误、并列主语、集合名词作主语、不定代词作主语、主语包含插入语和特定名词或短语作主语等。提供详细的改错解析，说明主谓一致的语法规则。

  
```
Please create a set of [数量] error correction exercises focusing on subject-verb agreement issues in English. Provide each exercise with its corrected version and detailed explanations for the corrections.
1. 指定任务：设计主谓一致的改错练习
2. 目标群体：未明确指定
3. 举例：未在提示中直接提供
4. 具体要求：涵盖多种主谓一致问题类型，并提供详细解析
```


## Part III. 听力篇

### 1. 听力材料改编

- 将阅读材料改编为听力材料，调整语言难度、风格和内容形式
    - **阅读转听力材料改编**：将书面语改编为口语形式，增强听力材料的真实性和交际性
  - **对话形式转换**：将原文改编为主持人对话形式，增加听力材料的吸引力
  - **难度调控**：根据需要（如欧框B1水平）调整语法复杂度、词汇难度和信息密度
  - **内容保留**：在改编过程中保留原文的关键信息和主要内容

  
```
Here is the material: [原始阅读材料]
Please convert this reading material into a listening material suitable for CEFR [级别] level learners.
1. 指定任务：将阅读材料转换为听力材料
2. 目标群体：明确指定语言水平（如CEFR B1级别）
3. 举例：可选择性提供改编示例
4. 具体要求：要求将书面语转为口语形式，可指定对话形式等特定风格
```
 
### 2. 听力习题设计

 
- 根据听力材料设计多样化的听力理解题目
  - **信息理解题设计**：设计单选/多选题、判断题，测试学生对听力材料中特定信息和细节的理解
  - **主旨大意题设计**：设计主观题或选择题，评估学生对听力材料整体内容的理解
  - **推断题设计**：设计需要学生基于听力材料进行合理推断的题目，测试更高层次的理解能力
  - **多样题型融合**：在同一练习中结合使用多种题型，全面测试听力理解能力

  
```
Please create listening comprehension questions based on the provided listening material including [数量] multiple-choice questions for information understanding, [数量] true/false question for information understanding, [数量] inference question, and [数量] subjective question to summarize the main idea. Please provide answers and explanation.
Here is the material: [听力材料]
1. 指定任务：基于听力材料创建不同类型的听力理解题
2. 目标群体：可在材料描述中指定目标学习者水平
3. 举例：可要求提供示例答案
4. 具体要求：明确指定不同类型题目的数量，并要求提供答案解析
```
 
### 3. 听力音频制作

 
- 将文本脚本转换为可用于听力教学的音频文件
   - **AI语音合成**：使用文本转语音(TTS)技术将文字脚本转换为MP3等音频文件
  - **参数调整**：根据教学需求调整语速、音色、口音和语调等参数
  - **停顿控制**：通过特殊标记(如<#0.5#>)添加特定时长的停顿
  - **多工具选择**：可使用讯飞配音、外研AI教师助手、[海螺AI](https://www.minimaxi.com/audio)、NaturalReader、TTSMaker、TTSMP3等多种工具

- **海螺AI工具操作步骤**：
  1. 将文字脚本粘贴到输入框
  2. 在"调试台"中设置音色、语速、声调等参数
  3. 点击"生成音频"
  4. 完成后点击右下角下载按钮获取MP3文件
 
### 4. 听力词表制作

 
- **基于听力材料创建词汇表，帮助学生预习和复习**
  - **听力生词表制作**：识别并列出听力材料中的生词、术语及特定语域的高频词汇短语
  - **词汇解析提供**：为每个词汇提供中文翻译、语法用法说明和相关背景知识
  - **命名实体解释**：为材料中出现的人名、地名、组织机构等提供简洁的英文解释
  - **词汇搭配补充**：针对特定词汇提供在相应语境（如新闻）中的常见搭配和例句

  
```
You are an English [具体领域] tutor, specializing in helping English learners. Your task is follow these steps:
1. Identify and list uncommon words, along with highly frequent words and phrases that are typical in [具体语域].
2. Provide the Chinese translation for each identified English term.
3. Clarify the grammatical usage of each term in English.
4. For named entities (like people, places, organizations) mentioned in the material, provide concise English explanations to clarify their relevance in the context.
Here is the material: [听力材料]
1. 指定任务：创建听力词表并提供多方面的词汇信息
2. 目标群体：英语学习者
3. 举例：可要求提供例句
4. 具体要求：识别特定类型的词汇，提供翻译、语法解释和背景信息
```


## Part IV. 口语篇

### 1. 小组辩论的立论与驳论内容促成

- 基于"产出导向法"的内容促成环节，为辩论活动生成多角度的正反理据
  - **辩论理据生成**：针对特定话题（如"人工智能生成的画作是艺术吗？"）从多个视角生成正反理据
  - **多视角引导**：从科技进步、后现代艺术理论、人类创造力、历史文化等多个角度提供论点
  - **论点配对**：为每个正面论点生成相应的反驳论点，帮助学生形成辩证思维

```
I need you to generate comprehensive arguments both supporting and opposing "[辩论话题]" from the viewpoints of diverse groups, in order to guide students in constructing arguments and counterarguments.
1. 指定任务：生成正反方的多角度论据
2. 目标群体：参与辩论的学生
3. 举例：未在提示中直接提供
4. 具体要求：从多个视角（如科技、艺术理论、人文等）提供论据
```
 
### 2. 音节接龙语言促成活动设计

- 通过音节知识学习改善语言产出，帮助学生掌握多音节单词的发音和拼写
  - **音节切分**：针对特定语义场（如"恶化"）生成多音节单词及其音节划分
  - **音节接龙活动**：基于切分好的音节，引导学生完成续接音节组词的任务
  - **针对性训练**：针对学生在多音节单词发音和拼写方面的困难进行有针对性的训练

  
```
Please generate a list of [数量] multisyllabic English words (comprising three or more syllables) that are associated with the notion of [主题]. Additionally, include the syllable divisions for each word.
1. 指定任务：生成特定语义场的多音节单词及音节划分
2. 目标群体：学习英语发音的学生
3. 举例：未在提示中直接提供
4. 具体要求：提供音节划分，使用连字符连接各音节
```
 
### 3. 听后续说任务设计

- 基于"续论"语言习得观的听后续说活动，结合听力理解与口语产出
  - **听力材料改写**：将阅读材料智能改写为欧框特定水平（如B2）的听力材料
  - **故事续说设计**：设计情境化的口语续说任务，引导学生创造性地补全和拓展听力材料
  - **拉平效应利用**：发挥听力理解与口语产出之间的拉平效应，提高口语表达能力

  
```
Please create a listening-speaking integrated continuation task suitable for CEFR [级别] level learners, based on the provided story. The listening part should be a [字数] word text, converted into an audio file with a [口音] English narration at a pace of [语速] words per minute. Additionally, include a continuation speaking sample that logically extends the story's theme from the listening segment. Here is the provided story: [故事内容]
1. 指定任务：创建听力-口语一体化的续说任务
2. 目标群体：明确指定语言水平（如CEFR B2级别）
3. 举例：提供续说的示例
4. 具体要求：指定听力材料长度、口音、语速和主题延续要求
```
 
### 4. 视后续说任务设计

- 基于图像的视觉输入进行续说活动，丰富输入模态
  - **AI图像生成**：使用文生图模型（如[通义万相](https://tongyi.aliyun.com/wanxiang/explore)）根据文本描述生成配图
  - **视觉引导口语**：利用生成的图片作为视觉刺激，引导学生进行续说活动
  - **故事配图生成**：可针对经典故事（如《金发姑娘和三只熊》）生成情境图片

- **通义万相使用步骤**：
  1. 将文字描述（如故事片段）作为提示语输入
  2. 保持提示语简洁，避免过长导致细节遗漏
  3. 如生成结果不满意，可多次尝试直至满意
  4. 将生成的图片应用于视后续说教学活动
 
### 5. 英语演讲稿修改和问答设计

- 辅助英语演讲比赛备赛，提高演讲技巧和应对即兴问答能力
  - **演讲稿修改**：从语法、不自然搭配、演讲语体等方面修改演讲稿
  - **语体调整**：将书面语表达改为更适合口头演讲的表达方式
  - **即兴问答设计**：基于演讲主题设计相关的即兴问答题目，帮助选手准备问答环节

  
```
Please review and improve the following speech manuscript titled "[演讲标题]" using in-text annotations. Focus on correcting any grammatical errors, awkward phrasings, and expressions that are not suitable for a speech. Additionally, create [数量] impromptu question-and-answer items based on the provided speech manuscript.
1. 指定任务：修改演讲稿并设计相关即兴问答题目
2. 目标群体：参加演讲比赛的学生
3. 举例：未在提示中直接提供
4. 具体要求：注明原文和修改后的文本，并提供可能的问答示例
```

## Part V. 阅读篇

### 1. 阅读材料编制

- 根据学生英语水平定制化阅读材料，解决阅读材料难度与学生英语水平不匹配的问题
  - **文本难度调整**：将原始文本调整为符合特定语言水平（如欧框B1水平）的材料
  - **语言简化**：简化短语、缩短句长、降低句法复杂度
  - **表达具体化**：将抽象表达转换为更具体的描述，使文本更易于理解
  - **句式调整**：简化时态和语态，避免过于复杂的句法结构

  
```
Please revise the provided text to match a CEFR-[级别] proficiency level, suitable for [目标群体] language learners. Use in-text annotations to highlight the modifications made.
1. 指定任务：将原文调整为特定语言水平的阅读材料
2. 目标群体：明确指定语言水平（如CEFR B1级别）
3. 举例：未在提示中直接提供
4. 具体要求：使用文内注释标明修改部分，便于教师对比原文和修改后的文本
```
 
### 2. 阅读习题设计

- 根据阅读材料设计多种类型的阅读理解题，全面评估学生的阅读理解能力
  - **多类型题目设计**：设计细节理解题、观点态度题、推理判断题和主旨大意题等多种类型题目
  - **答案解析提供**：为每道题目提供正确答案和详细的解析说明
  - **难度控制**：根据教学需求调整提示语，控制生成题目的难度水平
  - **针对性评估**：通过不同类型题目评估学生对文本的不同层面的理解能力

  
```
Please create [数量] multiple-choice reading comprehension questions based on the given text. These should include Detail, Attitude, Inference, and Main Idea Questions. Provide the correct answers with explanations for each question.
1. 指定任务：基于给定文本创建多选阅读理解题
2. 目标群体：未明确指定，可通过设定题目难度来调整
3. 举例：未在提示中直接提供
4. 具体要求：包括不同类型的题目，并为每道题提供答案和解析
```
 
### 3. 交互阅读游戏设计

- 利用大语言模型创建开放式、交互式的阅读游戏，提高学生阅读的趣味性和参与度
  - **交互式故事生成**：定制聊天机器人生成可交互的故事情境
  - **个性化设置**：允许设定文本风格、故事背景、主要人物等要素，使阅读材料更符合个人兴趣
  - **情节互动**：读者通过简单回复决定主人公行动，影响剧情走向
  - **词汇学习整合**：在故事中嵌入难词解释，帮助学生在情境中习得词汇

- **GPTs定制步骤**：
  1. 创建模型描述，设定角色（如Adventure Linguist）
  2. 说明功能（如在故事结尾解释难词、提供多种行动选择）
  3. 设定创作风格和互动方式
  4. 测试并调整模型响应
 
### 4. 识别争议焦点的观点促成活动设计

- 基于"产出导向法"理论，通过识别阅读材料中的争议焦点促进学生辩论和观点形成
  - **争议性材料生成**：针对特定话题（如"人工智能是否会取代人类工作"）生成包含多角度观点的阅读材料
  - **多层次争议点标注**：在句子、段落和篇章三个层面标注争议焦点
  - **辩论引导**：通过明确的争议点引导学生展开讨论和辩论
  - **观点形成促进**：帮助学生通过分析争议点形成个人观点

  
```
Please generate a controversial reading material based on the topic "[话题]" and highlight the points of contention at the sentence, paragraph, and discourse levels within the reading to guide students in engaging in debate.
1. 指定任务：生成包含争议点的阅读材料并标注争议焦点
2. 目标群体：未明确指定，可通过内容难度调整
3. 举例：未在提示中直接提供
4. 具体要求：在句子、段落和篇章三个层面标注争议焦点
```
 
### 5. 阅读教学思维导图绘制

- 通过思维导图可视化展示阅读材料的结构和核心内容，提升学生的理解和分析能力
  - **工具**: OpenAI 的 [Whimsical Diagrams](https://chatgpt.com/g/g-vI2kaiM9N-whimsical-diagrams)

  - **核心要素提取**：从阅读材料中提取主题句、重要事实、证据等核心要素
  - **结构化呈现**：以思维导图形式展示各要素间的逻辑关系
  - **层次清晰化**：通过主题分支和子节点清晰展示文本的层次结构
  - **思辨能力培养**：帮助学生厘清文本中的不同概念，培养分析和评价能力

  
```
Could you create a mindmap based on the provided text?
1. 指定任务：基于提供的文本创建思维导图
2. 目标群体：未明确指定
3. 举例：未在提示中直接提供
4. 具体要求：简洁明了，没有特定的额外要求
```
 
### 6. 阅读语篇主题词云图绘制

- 通过词云图直观展示阅读材料中关键词汇的频率分布，帮助学生把握文本核心
  - **关键词提取**：从阅读材料中识别并提取关键词汇
  - **频率可视化**：根据词汇出现频率或重要性设置不同字号和颜色
  - **停用词过滤**：去除无实际语义价值的常见词（如冠词、连词等）
  - **视觉引导学习**：通过视觉突出吸引学生注意力，激发讨论

  
```
Based on the provided text, please generate a word cloud. Please exclude the stop words from the word cloud.
1. 指定任务：基于提供的文本生成词云图
2. 目标群体：未明确指定
3. 举例：未在提示中直接提供
4. 具体要求：剔除停用词，以突出有实际语义价值的词汇
```
 

## Part VI. 写作篇

### 1. 不同语域同题文本生成

- 加强学生对正式和非正式英语的词句风格差异认识，解决学生写作中的语体或语域意识问题
  - **同题不同语域生成**：针对同一主题（如人工智能）生成正式和非正式两种风格的短文
  - **风格对比分析**：引导学生讨论两篇文章在词汇、语法、结构上的差异
  - **自我反思指导**：鼓励学生对照自己的写作，反思语域使用上的问题
  - **差异自动识别**：可通过提示让大语言模型直接比较两篇文章的词汇和语法差异

  
```
Could you write two [字数] essays on the topic "[主题]"? One should be in a formal style, and the other in an informal style.
1. 指定任务：就同一主题生成两种不同语域的文章
2. 目标群体：未明确指定
3. 举例：未在提示中直接提供
4. 具体要求：一篇使用正式风格，一篇使用非正式风格
```
 
### 2. 特定难度主题相关词句推荐

- 基于"产出导向法"的语言目标设计，为写作任务提供相关词汇和表达
  - **主题词汇生成**：为特定主题（如大学生创业）生成相关词汇和短语
  - **难度控制**：根据学习者语言水平（如欧框B2级别）控制词汇难度
  - **写作表达推荐**：提供与特定写作类型（如议论文）相关的表达方式
  - **双层列表设计**：分别列出主题相关词汇和写作类型相关表达

  
```
Please create a two-part list for CEFR [级别] level English learners. Part 1: List [数量] common words and phrases related to the topic of [主题]. Part 2: List [数量] expressions specifically beneficial for [写作类型] writing.
1. 指定任务：创建两部分词汇表，包括主题词汇和写作表达
2. 目标群体：明确指定语言水平（如CEFR B2级别）
3. 举例：未在提示中直接提供
4. 具体要求：分别列出特定数量的主题相关词汇和写作表达
```
 
### 3. 典型写作交际场景设计

- 基于"产出导向法"驱动环节的交际场景设计，创建真实有效的写作情境
  - **场景要素设计**：围绕四个要素（话题、身份、目的、场合）设计写作场景
  - **多场景生成**：为同一教学任务（如向外国朋友推荐中国电影）生成多个不同场景
  - **真实情境模拟**：设计贴近学生真实生活的交际情境，增强学习动机
  - **场景描述详细化**：为每个场景提供具体的背景描述和任务要求

  
```
Please create [数量] scenarios where [学习者身份] [交际任务], suitable for L2 writing exercises. Each scenario should include four essential elements, namely topic (information/issue, question/difficulty), purpose (to explain/clarify information, to persuade/argue a point of view), identity (identity of the speaker, identity of the listener) and setting (formal occasion, informal occasion).
1. 指定任务：创建包含四个基本要素的写作场景
2. 目标群体：二语写作学习者
3. 举例：提供场景示例以说明格式
4. 具体要求：每个场景必须包含话题、目的、身份和场合四个要素
```
 
### 4. 同义改写语言促成任务设计

- 基于"产出导向法"语言促成环节的同义改写练习，强化语言形式与意义的连接
  - **目标词汇生成**：围绕特定主题（如创新）生成目标词汇或短语
  - **简单段落创建**：基于相关主题（如中国科技创新）生成简单段落
  - **同义改写示例**：提供使用目标词汇进行同义改写的示例
  - **语言形式升级**：在改写过程中提升语言的复杂度和表达精确度

  
```
Please create [数量] related words or phrases appropriate for CEFR [级别] level students, focusing on the theme of "[主题]". Then, write a brief paragraph (under [字数] words) about [相关话题]. Instruct the students to rewrite this paragraph using the [数量] provided words or phrases. Additionally, provide an example of how the paragraph could be rewritten using these words or phrases.
1. 指定任务：创建目标词汇和需要改写的段落
2. 目标群体：明确指定语言水平
3. 举例：提供同义改写的示例
4. 具体要求：词汇应与主题相关，原段落和改写示例均需提供
```
 
### 5. 典型学生写作样本选择

- 基于"产出导向法"评价环节中"师生合作评价"的课前准备，选择适合评价的典型样本
  - **样本质量评估**：从多篇学生作文中选取质量适中、可改可评的作品
  - **选择理由分析**：解释选择特定样本的原因和适合评价的方面
  - **改进空间标注**：指出样本中存在的问题和可改进之处
  - **教学目标对照**：确保所选样本符合特定的教学任务和目标

  
```
Here are the writings of [数量] students. Please select [数量] pieces that represent typical samples and assess them in alignment with the objectives of the teaching task. Please present the reasons of selection and assessment.
A typical sample refers to a product of moderate quality that can be improved and assessed. Exceptionally excellent products have minimal areas for modification, while lower-quality products require extensive evaluation and editing, which may not be suitable for teaching focus.
1. 指定任务：从多篇学生作文中选择典型样本并评估
2. 目标群体：教师使用，用于课前准备
3. 举例：未在提示中直接提供
4. 具体要求：提供选择理由和评估结果，选择质量适中的样本
```
 
### 6. 议论文和说明文的读后续写设计

- 基于"续论"语言习得观的读后续写任务，帮助学生区分议论文和说明文的写作特点
  - **不同体裁材料生成**：围绕同一主题（如在线教育）创作议论文和说明文阅读材料
  - **续写任务设计**：设计相应的续写任务，要求学生采用相同体裁进行续写
  - **续写示例提供**：为每种体裁提供续写示例，展示该体裁的特点和结构
  - **体裁特点凸显**：在阅读材料中明确体现各体裁的典型特征和结构

  
```
Design two reading-writing integrated continuation tasks for CEFR [级别] level students, centered on the theme of "[主题]". The first task should focus on argumentative writing, while the second on expository writing. Ensure that each reading passage is around [字数] words. Additionally, provide an example of argumentative continuation writing for the argumentative reading passage. Similarly, provide an example of expository continuation writing for the expository reading passage.
1. 指定任务：设计两种不同体裁的读后续写任务
2. 目标群体：明确指定语言水平
3. 举例：提供两种体裁的续写示例
4. 具体要求：指定阅读材料长度，确保材料体现各体裁特点
```
 
### 7. 英语写作修辞的以续促学设计

- 通过读后续写任务促进学生英语写作修辞能力的提升
  - **修辞改写**：将原始文本（如童话故事）改写为包含特定修辞手法（如明喻、拟人）的版本
  - **修辞标注**：用特定格式（如XML标签）标注文本中使用的修辞手法
  - **续写引导**：设计续写任务，鼓励学生理解并应用相同的修辞手法
  - **创造性表达培养**：引导学生在保持逻辑连贯性的基础上创造性地使用修辞手法

  
```
Could you please rewrite the provided text to include [数量] instances of figure of speech, specifically, [修辞手法1] and [修辞手法2] (and annotate them in [标注格式])? Building on the revised text, please create a reading-writing integrated continuation task and ask learners to continue the story, encouraging them to fully understand the existing storyline and to extend it in a manner that is both creative and logically coherent.
1. 指定任务：改写文本并嵌入特定修辞手法，设计续写任务
2. 目标群体：英语写作学习者
3. 举例：提供包含修辞手法的改写文本
4. 具体要求：使用特定格式标注修辞手法，设计鼓励学生应用这些修辞的续写任务
```
 
### 8. 视读后续写任务设计

- 结合图像和文本的多模态"视读后续写"任务，提升阅读理解和写作表达能力
  - **文本配图生成**：为读后续写的阅读材料（如童话故事）生成配图
  - **关键情节可视化**：确保生成的图片能体现文本中的关键情节和细节
  - **多模态理解促进**：通过视觉和文字双重输入增强学生的理解
  - **图文结合提示**：通过提供精准的文本描述指导AI生成相符的图像

- **通义万相使用步骤**：
  1. 将阅读材料中的关键片段作为提示语输入
  2. 保持提示语简洁明了，聚焦于需要可视化的场景
  3. 如果生成结果不理想，可调整提示语后重新生成
  4. 将生成的图片与文本结合，设计"视读后续写"任务
 
### 9. 作文自动评阅

- 利用大语言模型的自然语言理解和生成能力对学生作文进行全面评阅
  - **多维度评阅**：从结构、连贯性、语法、风格、内容、创意、词汇和拼写等多个方面评估作文
  - **问题指出**：准确指出作文中的各类问题，如语法错误、结构不清等
  - **改进建议**：为每个问题领域提供具体的改进建议
  - **整体评价**：对作文整体质量给出综合评价，指明主要优势和不足

  
```
Please review the following student's writing, focusing on the aspects of structure and organization, clarity and coherence, grammar and syntax, style and tone, content and argument, creativity and originality, vocabulary and language use, as well as spelling and punctuation.
1. 指定任务：全面评阅学生作文
2. 目标群体：教师或进行自我评阅的学生
3. 举例：未在提示中直接提供
4. 具体要求：从多个方面评估作文，指出问题并提供改进建议
```


## Part VII. 翻译篇


### 1. 指定语汇翻译设计

- 基于"产出导向法"语言促成环节的指定语汇翻译练习
  - **指定语汇翻译练习**：引导学生使用特定目标词汇完成翻译任务
  - **关联词汇集中产出**：围绕重要意义（如"国际合作"）设计相互关联的词汇和表达
  - **双语对照练习**：提供英文目标词汇及其中文语境，引导学生进行汉译英翻译
  - **分级词汇设计**：根据学习者语言水平（如欧框B2）选择适当难度的词汇

  
```
Create [数量] phrases, each suitable for CEFR [级别] level English learners, centered on the theme of "[主题]". These phrases should be interconnected and contextually relevant for discussions about [主题]. Following that, devise a translation exercise from Chinese to English, focusing on the topic of [主题]. In this exercise, students will utilize the previously generated [数量] expressions, translating them to demonstrate their understanding of the theme and language proficiency.
1. 指定任务：生成指定主题的关联词汇短语并设计翻译练习
2. 目标群体：明确指定语言水平（如CEFR B2级别）
3. 举例：为每个生成的词汇提供短语示例
4. 具体要求：设计使用目标词汇的中译英练习题及参考答案
```
 
### 2. 汉英续译任务设计

- 基于"续论"语言习得观的翻译教学模式，将理解和产出紧密联系
  - **平行文本分段**：将文本分为阅读翻译部分（约2/3）和续译部分（约1/3）
  - **默译对照练习**：引导学生阅读原文、进行默译，并与标准译文对照反思
  - **读后续译练习**：在理解前部分内容的基础上，对后部分原文进行续译
  - **拉平效应利用**：通过前部分翻译对照学习，为后续部分续译提供语言支持

  
```
Translate [分数] of the provided text from the [考试名称/级别] [语言对] translation exam. Present the translation and the original text in parallel sentences. Leave [分数] of the original text untranslated for students to practice. Here is the text: [原文内容]
1. 指定任务：翻译部分原文，留下部分供学生续译
2. 目标群体：翻译考试（如CATTI二级）的备考学生
3. 举例：未在提示中直接提供
4. 具体要求：提供平行对照的原文和译文，并明确续译部分
```
 
### 3. 直译意译对比分析

- 展示直译和意译两种翻译方法的差异，帮助学生理解不同翻译策略的特点和适用场景
  - **直译版本生成**：保留原文的句式结构和表达方式，忠实传达原文的字面意思
  - **意译版本生成**：注重传达原文的整体意义和语气，使用目标语的自然表达方式
  - **对比学习**：引导学生分析两种译文的差异，理解不同翻译策略的优缺点
  - **适用场景讨论**：讨论何时应使用直译，何时应选择意译，培养翻译策略的选择能力

  
```
Please translate the provided [语言] passage into [目标语言], creating two distinct versions. For the first version, use a "literal translation" approach, where the translation closely follows the exact words and sentence structure of the original text. For the second version, use a free translation approach, focusing on conveying the overall meaning and tone of the passage rather than adhering strictly to the original wording and structure.
1. 指定任务：创建同一文本的直译和意译两个版本
2. 目标群体：翻译学习者
3. 举例：未在提示中直接提供
4. 具体要求：明确区分直译和意译方法，针对同一文本生成两种不同的译文
```
 
### 4. 口译重要概念解释

- 辅助译前准备中的专业领域知识学习，减轻口译准备工作量
  - **话题识别**：从口译材料中自动提取主要话题和讨论领域
  - **概念提取**：识别材料中出现的专业术语和关键概念
  - **概念解释**：为每个重要概念提供简明易懂的解释，帮助理解背景知识
  - **分步执行**：通过多个提问步骤逐步提取信息，提高生成内容的质量

  
```
Based on the excerpt provided from the [材料类型] transcript, can you determine the overarching subject of the discussion? Also, please list a few specific topics mentioned in this excerpt.
[提交文本后，继续提问]
Could you create a study sheet that introduces key technical concepts from this discussion? Aim for concise and simple explanations suitable for a general audience with basic or intermediate prior knowledge of the subject. Please focus on concepts that are essential for understanding the overarching topic.
1. 指定任务：识别口译材料主题并解释关键概念
2. 目标群体：口译学习者或译员
3. 举例：未在提示中直接提供
4. 具体要求：提供简洁易懂的概念解释，重点关注理解主题所必需的概念
```
 
### 5. 译前双语术语准备

- 为口译准备阶段建立专业领域的双语术语对照表，提高口译产出的准确性
  - **术语识别**：从给定材料中提取专业术语和技术词汇
  - **术语翻译**：提供每个术语的目标语言对应词
  - **参考资料辅助**：通过上传同主题的双语文本提高术语翻译的准确性
  - **拼音标注**：为中文术语提供拼音标注，帮助学习者掌握发音（可选）

  
```
Could you identify the technical terms related to the topic of the provided [文本类型] and translate them into [目标语言]? Please list the terms alongside their translations in two separate columns of a table.
[或者提供参考资料的版本]
Using the provided [语言1] and [语言2] documents, can you identify the technical terms related to their general topic? Please list these terms in a table with two columns: one for [语言1] terms and the other for their [语言2] equivalents.
1. 指定任务：创建双语术语对照表
2. 目标群体：口译学习者或译员
3. 举例：未在提示中直接提供
4. 具体要求：以表格形式呈现源语言术语及其目标语言对应词
```
 
### 6. 口译交传练习设计

- 利用大语言模型的多模态交互能力，创建更加真实的口译练习场景
  - **角色扮演**：大模型扮演英语母语者，学生扮演译员和其他交际角色
  - **场景模拟**：设置特定的交际场景和话题（如气候变化合作会议）
  - **真实口语互动**：通过手机端大模型的语音功能实现实时口语交流
  - **口译能力训练**：在真实交际需求下练习交替传译技能

- **多模态模型使用步骤**：
  1. 选择支持实时语音交互的模型（如GPT-4o、Gemini 2.0的Stream Realtime或智谱清言视频通话功能）
  2. 设置模型以识别语言切换（可使用"please go on"作为识别标记）
  3. 定义角色、场景和话题（如英语母语者讨论气候变化战略合作）
  4. 开始口译练习，模型将根据设定扮演角色并进行真实口语互动
 
---