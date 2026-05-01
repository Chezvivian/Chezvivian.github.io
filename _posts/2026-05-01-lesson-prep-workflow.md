---
title: '新课备课工作流'
date: 2026-05-01
tags:
  - thoughts
---

## 结论写在前面

**一、备课时间 baseline**

这是一次记录自己备课的测试。从五一前的周一到周四，四个工作日，最终还是没有找到可以在短期内（比如1天）轻松完成一节新课备课的路径。最主要的原因不是格式、图文调整，而是新课的知识部分，我没法在一天内完成对一节新内容的自洽和内化。换句话说，即使敲定了一个不错的三级大纲，在具体课程内容设计时，知识的范围和深度、引入的方式（包括案例项目的设计）、与同学们之间的交互思考，以及最后的实践反馈和拓展资料，都不是 AI 一两次生成能让我满意的。如果这些知识和设计让我觉得陌生、讲出来都很别扭、没有激情，那这就不会成为我的课件。

最终，四个工作日基本完成了 2 次课内容的准备，还不是完整版（第一节缺少课后延伸资料，第二节的课堂练习流程还没设计完整）。因此：**每次90分钟的新课，要达到有信心讲的程度，至少需要3个工作日来备课。这是本次测试的一个实证发现。**

**二、有效的备课工作流：三个阶段**

从流程上看，备课会使用多种工具，但经过这轮测试，已经沉淀出一个相对清晰的三阶段路径：

<div style="display: flex; flex-direction: column; gap: 0; margin: 28px 0; font-family: -apple-system, sans-serif;">
  <div style="display: flex; align-items: flex-start; gap: 16px;">
    <div style="display: flex; flex-direction: column; align-items: center;">
      <div style="width: 44px; height: 44px; background: #4f6ef7; border-radius: 50%; display: flex; align-items: center; justify-content: center; color: white; font-weight: bold; font-size: 15px; flex-shrink: 0;">A</div>
      <div style="width: 2px; height: 28px; background: #d0d8ff;"></div>
    </div>
    <div style="flex: 1; background: #f5f7ff; border-radius: 10px; padding: 16px 20px; margin-bottom: 0;">
      <div style="font-weight: 700; font-size: 15px; margin-bottom: 6px; color: #2d3a8c;">第一阶段：大纲与内容框架</div>
      <div style="font-size: 14px; color: #444; line-height: 1.7;">使用目前能用到的最好的大模型来做「大脑」，通过明确的提示词确认知识模块和大致的案例节奏，得到初步的内容结构。如有不满意的地方，可以修改案例和内容范围。</div>
      <div style="margin-top: 10px; font-size: 13px; color: #7080cc;">工具：Claude Sonnet 4.6（主力）· Opus 4.7（中断时补充）· DeepSeek-V4-Pro</div>
    </div>
  </div>
  <div style="display: flex; align-items: flex-start; gap: 16px;">
    <div style="display: flex; flex-direction: column; align-items: center;">
      <div style="width: 44px; height: 44px; background: #34a06e; border-radius: 50%; display: flex; align-items: center; justify-content: center; color: white; font-weight: bold; font-size: 15px; flex-shrink: 0;">B</div>
      <div style="width: 2px; height: 28px; background: #b0dfc8;"></div>
    </div>
    <div style="flex: 1; background: #f2fbf7; border-radius: 10px; padding: 16px 20px;">
      <div style="font-weight: 700; font-size: 15px; margin-bottom: 6px; color: #1a6644;">第二阶段：课件呈现与课堂动线设计</div>
      <div style="font-size: 14px; color: #444; line-height: 1.7;">将修改过的内容大纲喂给 PPT 生成工具，或转为 HTML 演示文件后筛选页面、手动编辑、截图保存，再整合到个人 PPT 模板里。这里的「呈现」也包括对课堂交互和具体活动的设计。PPT 抽卡了两三版，HTML 抽了四版以上，整体来说更倾向于 HTML 路径：生成快、文件小、后期可自己修改，定制感更好。</div>
      <div style="margin-top: 10px; font-size: 13px; color: #4a9470;">工具：AIPPT · Cursor（HTML）· DeepSeek-via-Sider（HTML）</div>
    </div>
  </div>
  <div style="display: flex; align-items: flex-start; gap: 16px;">
    <div style="display: flex; flex-direction: column; align-items: center;">
      <div style="width: 44px; height: 44px; background: #e0952a; border-radius: 50%; display: flex; align-items: center; justify-content: center; color: white; font-weight: bold; font-size: 15px; flex-shrink: 0;">C</div>
    </div>
    <div style="flex: 1; background: #fffbf2; border-radius: 10px; padding: 16px 20px;">
      <div style="font-weight: 700; font-size: 15px; margin-bottom: 6px; color: #7a5010;">第三阶段：课堂练习附属资料</div>
      <div style="font-size: 14px; color: #444; line-height: 1.7;">准备翻译质量评估案例和 Excel 表格、项目管理 Word 文档等练习材料。呈现给学生的是 Office 全家桶格式，但生成时先让 Cursor 做 md 和 csv 文档，更快、更小、更灵活，最后再转换。</div>
      <div style="margin-top: 10px; font-size: 13px; color: #b07830;">工具：Cursor（md/csv 生成）· Office 全家桶（最终格式）</div>
    </div>
  </div>
</div>

---

## 缘起

### 人工智能+X 的新课

"人工智能+X"作为贸大研究生的公共必修课，已经开设过三个学期。我和崔老师都已经上了两轮，每学期内容都有较大变化——除了排课给的课时多少不同（有的学期2次课，有的4次课），针对不同的授课对象，包括本学院的外国语言学与应用语言学、英语、口译、笔译专业，以及前两学期对外汉语、小语种专业的学生，每轮上课的内容都会针对性调整，包括 AI 工具使用的场景和应用难度。

两轮教学下来，总结出之前的课堂问题：

1. **第一轮**：设计的 AI 应用难度过高。当时使用阿里云的 Python 平台，让同学们用 AI 工具设计语料提取和语料分析的代码。学生的学习难点在于：对 Python 语言本身的陌生感、对阿里云代码平台的陌生感、对语料分析场景的陌生感——三重陌生叠加，实践难度大，学习效果不佳。

2. **第二轮**：转向 AI 应用的知识 + Sketch Engine 语料库创建与对齐，以及用 AI 智能体管理个人术语库。因为去掉了 Python 部分的挑战，聚焦于常见软件 + AI 使用，学生反馈有所提升。

这学期的第三轮，我重新设计了全部4次课的内容。最主要的原因是：崔老师此次也是4次课，是我的前置课程，他的内容已经覆盖了译前、译中、译后和字幕配音实战，非常完整。如果我再对语料库、术语库的管理赘述，意义不大——索性抛开翻译操作中具体的 AI 使用，转向广义的**翻译项目管理**。

项目管理能力是这两年我特别想引导学生关注的地方。虽然本科甚至 MTI 学生对项目管理会感到陌生，但这偏偏正是学校教育和公司职业教育中可能脱节的部分。在本地化行业的实习工作中，我发现 project management 是公司非常看重、对职业发展有至关重要作用的一种"元能力"。如果能在 AI 辅助下，让学生沉浸式地理解这种工作环境和对能力的要求，对教学、对学生的学习和未来工作都应该有好处。

### 为什么要记录这次备课

这次记录新课备课工作流，有两个目的：

1. **呈现全流程，蒸馏出高效路径。** 把从目标到实现的全流程——弯路、直路——都记录下来。目标是在完成备课时回看，确保完成了最初的备课目标，同时蒸馏出效率更高的工作流。

2. **为明年的新课做演练。** 今天对4次课的备课是一个演练，为明年本科全新16周课程《语言数据科学》做准备。开一门全新的课是一个巨大的挑战，包括确定课程范围、模拟目标学生、准备课堂知识和案例练习。其中知识的筛选和适配、工具的选择和测试、案例设计，都是可更新的变量。

---

## 备课目标

### 本学期的课次安排

<div style="display: flex; align-items: stretch; gap: 0; margin: 28px 0; font-family: -apple-system, sans-serif;">
  <div style="flex: 1; background: #f0f4ff; border-radius: 10px 0 0 10px; padding: 18px 16px; border-left: 5px solid #4f6ef7;">
    <div style="font-weight: 800; color: #4f6ef7; margin-bottom: 6px; font-size: 13px; letter-spacing: 1px;">第六节</div>
    <div style="font-size: 14px; font-weight: 600; margin-bottom: 8px; line-height: 1.5;">语言服务交付与项目管理基础</div>
    <div style="font-size: 12.5px; color: #666; line-height: 1.6;">建立全局认知：项目从哪来、到哪去、谁来管、AI 改变了什么</div>
  </div>
  <div style="display: flex; align-items: center; padding: 0 4px; background: #e8eeff; color: #8898e8; font-size: 18px;">›</div>
  <div style="flex: 1; background: #f0f8f4; padding: 18px 16px; border-left: 5px solid #34a06e;">
    <div style="font-weight: 800; color: #34a06e; margin-bottom: 6px; font-size: 13px; letter-spacing: 1px;">第七节</div>
    <div style="font-size: 14px; font-weight: 600; margin-bottom: 8px; line-height: 1.5;">AI辅助本地化质量管理进阶</div>
    <div style="font-size: 12.5px; color: #666; line-height: 1.6;">切入核心价值：质量如何定义、度量、用 AI 检测和保障</div>
  </div>
  <div style="display: flex; align-items: center; padding: 0 4px; background: #e6f4ed; color: #88c8a8; font-size: 18px;">›</div>
  <div style="flex: 1; background: #fff9f0; padding: 18px 16px; border-left: 5px solid #e0952a;">
    <div style="font-weight: 800; color: #e0952a; margin-bottom: 6px; font-size: 13px; letter-spacing: 1px;">第八节</div>
    <div style="font-size: 14px; font-weight: 600; margin-bottom: 8px; line-height: 1.5;">翻译资产的战略管理</div>
    <div style="font-size: 12.5px; color: #666; line-height: 1.6;">追问质量根基：术语库、记忆库、风格指南如何体系化管理并产生回报</div>
  </div>
  <div style="display: flex; align-items: center; padding: 0 4px; background: #fdf3e4; color: #d0b080; font-size: 18px;">›</div>
  <div style="flex: 1; background: #fdf0f0; border-radius: 0 10px 10px 0; padding: 18px 16px; border-left: 5px solid #d94f4f;">
    <div style="font-weight: 800; color: #d94f4f; margin-bottom: 6px; font-size: 13px; letter-spacing: 1px;">第九节</div>
    <div style="font-size: 14px; font-weight: 600; margin-bottom: 8px; line-height: 1.5;">AI工作流与风险管理</div>
    <div style="font-size: 12.5px; color: #666; line-height: 1.6;">收束工程实践：将项目、质量、资产编织进可执行工作流，并管控风险</div>
  </div>
</div>

### 核心设计点

每节课的备课都围绕以下三个模块展开：

1. **课程目标 + 目标图谱**
2. **课程组成部分**
   - 知识：行业知识 + 技术知识，说明重难点
   - 案例：讲解背景、实施策略、目的和方法
   - 演练：技术操作、小组讨论策略
3. **使用的工具**
   - AI 工具、接口、流程
   - 软件、截图、视频

---

## 备课工作流记录

### 今天的参考资料

这次备课参考了两个来源：

**① 学校新上的"AI好课·研究生智慧课程平台"**

本学期在《计算机辅助翻译AI+》和《本地化翻译》课上已经使用，但还没有彻底摸清使用逻辑和好处，只是先推荐了平台上的 AI 工具箱给学生。今天会借助学校之前的培训视频、知途好课视频号上的教学视频，一起深度学习平台的功能。

**② 影视飓风最新的工作流讲解视频**

Tim 讲了他们2026年与2024年相比的全新工作流，包括其中 AI 分别作为辅助和主导的部分。他们的前期脚本分镜、后期影视制作的逻辑，有一部分和备课有异曲同工之妙。借助一个成熟创业影视公司的经验，来参考 AI 使用的深度和范围，更新使用方法，同时祛魅一些过度宣传。

---

### 第一步：生成课程目标

**方法**：把课程背景、我的教师身份、前置课次的安排等信息告诉 AI，并给出已经敲定的课次主题和目录，要求生成有课次之间联系、且和崔老师内容衔接的课程目标。

**AI工具**：DeepSeek-V4-Pro（DeepSeek V4 刚发布，趁机试一试）

**结果**：AI 给出了很详细的课程目标体系文档（放在[这里](../files/posts/AI+X_goals.md)，可以点开看），对我来说有用的信息是：

- **整体定位**：前序课程聚焦于"译者视角的 AI 应用"（译前准备、译中辅助、译后编辑、字幕与配音实战），核心是培养学生在 AI 辅助下完成翻译任务的能力。本模块（第6–9节）切换到"管理者视角的 AI 应用"，从项目交付、质量管控、资产沉淀、流程工程四个维度，培养学生管理翻译业务的能力。
- **各节逻辑**：第六节建立全局认知，第七节切入核心价值维度，第八节追问质量的根基，第九节收束到工程实践。这个逻辑链条跟我之前做大纲时的思路基本一致。

**Comments**：初步的工作，AI 做的还可以。目标部分的思路跟我之前的大纲基本一致，相当于已经把课程内容和逻辑捋顺。这一步没问题的话，就可以进入知识部分了。

---

### 第二步：扩展知识内容

**方法**：知识是一个很重要的模块，需要专业、权威的信息做支撑，同时又不能太教科书——因为课堂的下半段就是实践和练习。重点是：找到权威的知识来源，找出本节课的重难点，最后把它梳理成图文并茂的课件。这一步要一节课一节课地来，因为每节课的内容需要扩展收缩，有较多的人工介入。

**AI工具**：DeepSeek 之外，同步使用了 Sider 的 AI PPT 功能。今天把刚才的课程目标上传，写了一些 prompt，发现居然能弹出很具体的下一步指示，做个参考。

**结果**：两个工具分别生成的知识大纲都契合三级目录，没有偏离。但以目录为基础生成的内容，很难在一轮对话中给出我想要的知识结构——**这是第一个需要人工多轮介入的地方**。

不过 AIPPT 有一个亮眼之处：在课件最初给出了一个可视化的学习路线图，比我常用的 PPT 摘要缩放定位要更清晰一点，因为加上了各个部分的具体作用，相当于有了上下文，这个不错。

---

### 第三步：PPT 制作抽卡

PPT 是我一个矛盾的点。近几年已经形成了自己的 PPT 风格：简约 + 简单的撞色，加一些形状，以及深度使用 SmartArt。这套做法可以比较快速地把内容形成图文形式，对我来说是高效的。但偶尔会觉得稍显幼稚，审美有点疲劳——而且想在 AI 生成的基础上增加更 fancy 的图片，往往意味着要增加很多抽卡时间，且 AI 生成 PPT 的内容和形式好往往只能占一头，得不偿失。

这次测试的工具对比如下：

<div style="display: flex; gap: 14px; margin: 24px 0; font-family: -apple-system, sans-serif; flex-wrap: wrap;">
  <div style="flex: 1; min-width: 180px; background: #f5f7ff; border-radius: 10px; padding: 16px 18px; border-top: 4px solid #4f6ef7;">
    <div style="font-weight: 700; font-size: 15px; margin-bottom: 8px;">AIPPT</div>
    <div style="font-size: 13.5px; color: #555; line-height: 1.7; margin-bottom: 10px;">图文效果不错，但生成页数总是10–12页，吞掉了很多内容，需要手工增加，麻烦。</div>
    <div style="font-size: 12.5px; color: #34a06e; margin-bottom: 3px;">✓ 视觉效果较好</div>
    <div style="font-size: 12.5px; color: #d94f4f;">✗ 内容完整性不足</div>
  </div>
  <div style="flex: 1; min-width: 180px; background: #f3f5ff; border-radius: 10px; padding: 16px 18px; border-top: 4px solid #6c72f7;">
    <div style="font-weight: 700; font-size: 15px; margin-bottom: 8px;">DeepSeek（via Sider）</div>
    <div style="font-size: 13.5px; color: #555; line-height: 1.7; margin-bottom: 10px;">在 Sider 里调用，生成的是 HTML 文档，格式效果不行，但大模型不错，生成的内容质量高，可以用来二次制作 PPT。</div>
    <div style="font-size: 12.5px; color: #34a06e; margin-bottom: 3px;">✓ 内容质量高</div>
    <div style="font-size: 12.5px; color: #d94f4f;">✗ 格式视觉效果差</div>
  </div>
  <div style="flex: 1; min-width: 180px; background: #f8f8f8; border-radius: 10px; padding: 16px 18px; border-top: 4px solid #bbb;">
    <div style="font-weight: 700; font-size: 15px; margin-bottom: 8px;">百度文库</div>
    <div style="font-size: 13.5px; color: #555; line-height: 1.7; margin-bottom: 10px;">审美一般，体验不佳，已弃用。</div>
    <div style="font-size: 12.5px; color: #d94f4f; margin-bottom: 3px;">✗ 审美风格不符</div>
    <div style="font-size: 12.5px; color: #999;">已弃用</div>
  </div>
</div>

**本次 PPT 制作的有效路径：**

1. 先和高阶思考型 AI 对话，给出课程设计的结构、本章主题、上下文，要求生成 PPT 内容大纲，得到初步内容结构。如有不满意的地方，修改案例和内容。
2. 将大纲喂给一个专注于 PPT 制作的 AI 工具（能追问具体定位、呈现方式的那种），要求严格按照大纲制作，得到初步未适配的 PPT，再筛选内容、删掉多余页面。
3. 对保留的重点页面进行编辑、增加动画效果，最后整合到个人的 PPT 模板里，组成结构化内容。

---

### 第四步：案例和演练

**方法**：从知识部分过来，基本上已经用 AI 形成了一版 PPT，知识性内容经过编辑完成。剩下的是结合实操：模拟案例和演练，同时增加具体的 tutorial（软件使用截图、流程引导等）。

**中途的思路变化**：

> 暂停。不再以知识为核心发展出次要的练习，而是以项目式任务为核心（PBL），从项目中需要的能力引出核心知识。这是今年可以尝试的新路径，也许是备课的破局点，而且可以打破之前对于课堂无聊、纯知识性内容太多的忧虑。
>
> ——实际 AI 脚本产生效果不佳，不如之前的知识大纲稳健。此思路弃用。

**新思路落地**：

1. 生成结构合理、课程设计完整的 md 课程大纲文件。
2. 用 Cursor 生成 HTML 课件文档，辅以课件风格（配色、字号等），从 HTML 中手动导出使用的页面，或者全部导出为 PDF 或 PNG 图片集合（进阶想法是加入基本的淡入动画）。
3. 在 Cursor 中形成课件风格的 skill，确保标题、字号、页码等格式一致。此处存疑：虽然使用了 skill，生成效果居然还不如"野生的"，所以可能之后再多次抽卡。另外尝试了借用网上很火的 zarazhang 的 HTML skill，但预装内容太多，在 Cursor 中两次生成都没完成——课程类 PPT 内容太多，输出 token 可能超了，实用性有限。
