---
layout: single
title: "实证研究数据处理的过程标准化探索"
---

<div style="margin-bottom: 2em;">
  <a href="/podcasts/" style="color: #007acc; text-decoration: none; font-weight: 500;">← 返回 Vivian's 播客小镇</a>
</div>

* TOC
{:toc}

## 写在前面 (2025-7-22)

这个频道的出发点是，记录下我处理GLOC_24眼动实验数据的全过程。通过观察、分解数据处理、建模的全过程，描绘出一个可拓展到同类实证研究的R代码框架。概览的思路是：

1. 数据导入、清洗 --> 
2. 筛选出需要的列数据，整理排列为标签完整的行、列数据 --> 
3. 针对各个研究问题，存储各自所需数据的完整数据框 -->
4. 根据自变量、因变量的数据性质，划分几种主流的线性模型构建方法。每个方法包括数据的描述性统计、分布分析、固定和随机效应变量确认、初步拟合、拟合优度检验、数据变换、再次拟合、对比拟合优度、输出较优模型的统计结果。-->
5. 制图，使用 ggplot，根据数据特性，制作有区分度的图表。后期调整重点是比例、坐标轴值域、配色外观等。-->
6. 统计结果和制图的公式保存、结果输出，且全流程保存为 rmd 文档，写明过程，以便回溯。

这个概览的思路是和以前实验数据处理一脉相承的事情，虽然繁琐，但是并不陌生。然而这次想做的过程标准化探索，是借助AI大模型的力量，对已有的流程再做一次结构化处理。思路1：以工作流为基础，构建出帮助处理数据的智能体，以AI agent 为重要辅助，核心是搭建工作流和调用 LLM；思路2：以数据处理的逻辑块为基础，构建出半固定的流程界面，将AI 辅助固定在具体的任务上，目标产品是可视化的交互式网站界面，用户可以直接上传所有实验数据，在流程的引导下，半自动地描述数据、选择处理选项，完成全流程。

思路2 是我更想做到的，一个类似于“傻瓜式”的一站式数据处理网站，极大地有利于翻译实证研究者快速得出实验结果。这种形式的前驱是 Michael 那一套 Translog 数据放在 YAWAT 平台上一键导出的效果，但是 YAWAT 的数据是直接从 Translog 导出的，因此数据是从闭源到开源。而思路2想做的是从半开源（需要符合一定的数据特性，再加以描述）到闭源的效果。Translog 和 YAWAT 的缺点很明显，从数据报错到手工对齐的繁琐，再到导出的半原始数据，都造成了很多的不方便。我想做的新工具不见得能实际上产生更好的效果，但是，试一试吧，谁知道呢？

## 第一节：眼动研究数据处理全流程 Overview 

这一节是对于眼动数据处理全流程的梳理：

使用 NotebookLM 制作了流程的讨论对话，用来加深印象。

<audio controls style="width: 100%; max-width: 600px; margin: 2em 0;">
  <source src="/files/podcasts/empirical-data/眼动研究数据处理全流程.wav" type="audio/wav">
  您的浏览器不支持音频播放。
</audio>

### Part 1 数据导入与预处理
1. **环境配置**
   - 设置系统区域设置（`Sys.setlocale('LC_ALL', 'Chinese')`）
   - 设置工作目录
   - 加载必要的R包（数据处理包、统计分析包、可视化包等）
   - 加载自定义函数（如`readTobiiTables.R`）
   
2. **原始数据导入**
   - 导入眼动数据（使用`readFixationSummary`函数处理Tobii导出的数据）
   - 导入按键数据（keystroke数据，使用`calcKeystroke`函数）
   - 导入NASA认知负荷量表数据
   - 导入翻译产品（译文）数据

3. **数据合并**
   - 将眼动数据和按键数据合并
   - 将合并后的数据与NASA评分结合
   - 添加必要的列标识符（如参与者ID、文本类型、通道等）
   - 将处理后的眼动列数据整合到一个数据框中

### Part 2 数据清洗与转换
1. **异常数据处理**
   - 移除不正确的响应数据（如脚本中移除了特定的会话：P14_H01_double, P18_H02_double等）
   - 移除不准确的会话数据
   
2. **数据分区**
   - 根据研究问题（RQ1、RQ2）分隔数据
   - 根据文本类型（H文本、V文本）分隔数据
   - 根据翻译经验（专业/新手）分隔数据

3. **创建兴趣区域（AOI）分析数据框**
   - 将ST（源文本）、TT（目标文本）、视频区域数据整合
   - 计算各兴趣区域的注视百分比

### Part 3 统计建模与分析
1. **描述性统计**
   - 查看各变量的描述性统计指标
   - 检查数据分布情况

2. **构建统计模型**
   - 线性混合模型（lmer）用于连续变量
   - 广义线性混合模型（glmer）用于计数数据（泊松分布、负二项分布）
   - 对正态性和离散性的检验与调整

3. **模型评估与优化**
   - 对比不同模型（AIC、R²、离散性）
   - 进行数据转换（如log转换）以满足模型假设

### Part 4 结果可视化与输出
1. **结果可视化**
   - 绘制预测效应图
   - 创建比较图表（如箱线图、直方图）
   - 组合多图展示

2. **结果汇总与保存**
   - 输出统计模型结果表
   - 保存图表和数据

## 第二节：Part I 原始数据类型和整合

和 Claude 聊了一下，把原始数据类型列出来，并给出处理思路，再导入到 napkin 中生成一个脑图，如下。

### 处理思路

<img src="/files/podcasts/empirical-data/1_data_type_process.png" alt="思路：数据类型和处理思路" width="500"/>  


### 数据类型

在2024年12月整月收集的实证数据，主要分为以下四类：

1. 眼动IA report (Eyelink导出)：包含每个被试、每个试次、每个兴趣区（IA）的汇总指标，如注视时长、首次注视时间等。
2. 被试访谈录音 (已转为文字)：包含被试的主观反馈，如困难度、策略描述等。
3. 被试译文文本：可用于评估翻译质量。
4. 被试背景信息文件 (Excel表格)：包含人口学信息、语言水平等。

其中最核心、影响实验结果的是第一类的眼动兴趣区数据，通常可以最快出结果（按照常规的混合效应线性模型构建方法），决定研究问题是否被验证，是否出了显著性结果。

之后的被试主观数据、译文质量两类数据的处理，以往需要非常多的手动工作，因此旷日持久，且结果不一定显著。但是，今年这次的流程创新有可能可以解决这个问题。

一方面是效率提高——访谈录音可以自动转录，且用统一标签的方法，快速提取有效信息，过程中可以使用LLM来协助；

另一方面译文质量的评估，以往是个老大难问题。因为翻译专家对译文的评估，即使基于同一个标准，比如 MQM, FAR等专业质量评估框架，个体的主观性往往非常强，很难形成较高的评分者信度。所以，今年也许可以尝试COMET等人工智能辅助评分的方法，让人工智能用统一的方法来评估质量。即使大概率会被质疑，但是效率、质量的平衡和统一，一定会有价值和意义。

### 各类数据的整合

为进行混合效应模型分析，需要将清洗后的多源数据整合到一张主表中。

目标形式：

- 混合效应模型通常每一行是一次被试-材料（或被试-材料-区域，依据分析层级）的观测。
- 核心变量包括：Subject（被试ID）、Text（材料/句子/段落ID）、Task (任务类型)、IA（如果按区域分析）、关键眼动指标（因变量）、以及协变量（如背景信息、访谈评分、译文评分等）。

整合方法：

- 主表结构选择：以‘被试-材料-IA’为主键，一份长表。
- 主表来源：以眼动IA report清洗得到的表为基础，因为它包含了最细致的观测层级。
- 数据合并：
    - 对于被试级别的数据（如背景信息、访谈评分），使用Subject作为匹配键进行合并（merge）。
    - 对于材料级别的数据（如译文评分），使用Subject-Item作为匹配键进行合并。
- 预期总表结构：
    - | Subject | Text | Task | IA | GazeDuration | ... | Accuracy | Fluency | InterviewDifficulty | LanguageLevel |


流程小结：
1. 逐份数据文件清理、整理成长表结构。
2. 用merge/join的方式合并为一份总表，确保主分析变量全部齐全。
3. 对关键分析维度进行检查（如每个被试、每个材料在每个IA下是否都齐全）。
4. 变量标准化/正态变换（如必要），为选择合适的混合效应模型做最后准备。



## 第三节 Part 2 数据清洗、数据框整理、准备过程

### A. 数据清洗
1. **异常值处理**
   - 通过`excludeOutlier`函数移除离群值，基于z-score方法（> 2.5标准差）
   - 脚本中使用如下代码移除特定的错误响应：
     ```R
     process_clean <- process_all[-c(which(process_all$Label == "P14_H01_double"), 
                                    which(process_all$Label == "P18_H02_double"),
                                    which(process_all$Label == "P22_H02_single"),
                                    which(process_all$Label == "P07_H01_double"),
                                    which(process_all$Label == "P26_H01_single")),]
     ```

2. **缺失值处理**
   - 设置默认值（如单轨道条件下视频区域的注视时长设为0）
     ```R
     FixationCols$FixNum_Video[which(FixationCols$Channel == "single")] <- 0
     FixationCols$FixDur_Video[which(FixationCols$Channel == "single")] <- 0
     ```

3. **数据分类与标记**
   - 根据参与者专业程度分组
     ```R
     RQ1_pro <- RQ1_data[c(which(RQ1_data$Part == "P04"),
                         which(RQ1_data$Part == "P06"),...),]
     RQ1_nov <- RQ1_data[-c(which(RQ1_data$Part == "P04"),
                          which(RQ1_data$Part == "P06"),...),]
     ```
   - 添加文本类型标签
     ```R
     RQ1_data$Text_type[which(RQ1_data$Text_type == "H")] <- "Talking head\n(high level)" 
     ```

### B. 数据框整理
1. **计算关键指标**
   - 总注视时长与注视点计算
     ```R
     FixationCols$TotalFixDur <- FixationCols$FixDur_ST + FixationCols$FixDur_TT + FixationCols$FixDur_Video
     FixationCols$TotalFixNum <- FixationCols$FixNum_ST + FixationCols$FixNum_TT + FixationCols$FixNum_Video
     ```
   - 计算平均注视时长
     ```R
     FixationCols$AvgFixDur <- FixationCols$TotalFixDur/FixationCols$TotalFixNum
     ```
   - 计算各兴趣区域的注视百分比
     ```R
     FixationCols$Ratio_ST_Fix_dur <- FixationCols$FixDur_ST/FixationCols$TotalFixDur
     ```

2. **数据转换为长格式用于可视化**
   ```R
   AOI_summary <- pivot_longer(process_clean[,c(1:4,10:12)], 
                              cols = c("FixDur_ST", "FixDur_TT", "FixDur_Video"), 
                              names_to = "AOI", values_to = c("FixDur"))
   ```

3. **数据过滤**
   - 根据研究问题过滤数据
     ```R
     RQ1_data <- process_clean[which(process_clean$Channel == "double"),]
     RQ2_data <- process_clean[which(process_clean$Text_type == "H"),]
     ```

### C. 数据准备
1. **计算多种眼动指标**
   - 注视时长
   - 注视次数
   - 平均注视时长
   - 注视时长占比
   - 注视次数占比

2. **计算按键指标**
   - 总按键次数
   - 插入次数（Insertion）
   - 删除次数（Deletion）
   - 暂停次数与时长（阈值：300ms, 1000ms）

3. **数据整合**
   - 将眼动数据、按键数据和NASA评分整合

## 第四节 Part 3 统计建模与数据分析

### Step 1. 数据特征分析
1. **分布检验**
   - 使用`shapiro.test`检验数据是否符合正态分布
   - 检查直方图识别分布形状
   - 使用箱线图检测离群值

2. **数据转换**
   - 对非正态分布数据进行log转换
     ```R
     TotalFixDur_2 <- lmer(log(TotalFixDur) ~ Text_type + (1|Part), data = RQ1_data)
     ```
   - 使用Box-Cox转换寻找最优变换参数
     ```R
     TotalFixDur_box <- optim.boxcox(TotalFixDur_0, data = RQ1_data, find.in.range = c(-2,2))
     ```

### Step 2. 模型构建
1. **线性混合模型（连续型因变量）**
   - 对注视时长等连续型数据使用lmer模型
     ```R
     TotalFixDur_1 <- lmer(TotalFixDur ~ Text_type + (1|Part), data = RQ1_data)
     ```
   - 加入随机效应考虑参与者差异
     ```R
     RQ2_AvgFixDur_2 <- lmer(TotalFixDur/TotalFixNum ~ Channel + (1|Part) + (1|Text_ID), data = RQ2_data)
     ```

2. **广义线性混合模型（计数型因变量）**
   - 对注视次数等计数数据尝试泊松分布
     ```R
     TotalFixNum_glm_1 <- glmer(TotalFixNum ~Text_type + (1|Part), data = RQ1_data, family = poisson())
     ```
   - 考虑过离散问题，采用负二项分布
     ```R
     TotalFixNum_glm_2 <- glmer.nb(TotalFixNum ~Text_type + (1|Part), data = RQ1_data)
     ```

3. **模型检验与选择**
   - 使用simulateResiduals检验离散性
     ```R
     sim_TotalFixNum_glm_1 <- simulateResiduals(TotalFixNum_glm_1, refit=T)
     testDispersion(sim_TotalFixNum_glm_1, plot = T)
     ```
   - 比较AIC/BIC值选择最优模型
     ```R
     tab_model(TotalFixDur_1, show.aic=T, show.stat = T)
     tab_model(TotalFixDur_2, show.aic=T, show.stat = T)
     ```

### Step 3. 效应检验
1. **主效应与交互效应**
   - 检验文本类型效应
   - 检验通道效应（单模态vs多模态）
   - 检验文本类型与通道的交互效应

2. **事后检验**
   - 使用emmeans进行简单效应分析
     ```R
     pairs(emmeans(RQ2_fixdur_ST_all_2, ~ Channel | Text_type))
     ```

## 第五节 Part 4 数据输出与可视化

### Step 1. 统计结果输出
1. **表格输出**
   - 使用tab_model函数生成模型统计表
     ```R
     tab_model(TotalFixDur_2, show.df = T, show.se = T, show.aic=T, show.stat = T)
     ```
   - 使用kable和kableExtra包格式化表格
     ```R
     save_kable(kable(RQ1_describe,format = "html", booktabs = TRUE) %>% kable_classic(),
         "../!Submission Drafts/Tables/RQ1_summary.html", bs_theme= "simplex")
     ```

2. **效应值提取**
   - 从模型中提取效应大小与显著性
     ```R
     FixDur_AOI_stat <- rbind(FixDur_ST_stat,FixDur_TT_stat,FixDur_video_stat) 
     FixDur_AOI_stat[,2:7] <- round(FixDur_AOI_stat[,2:7], digits = 2)
     ```

### Step 2. 可视化
1. **效应图**
   - 使用plot_model绘制预测效应
     ```R
     TotalFixDur_2_plot <- plot_model(TotalFixDur_2, type =c("pred"),terms = c("Text_type"),
                              axis.title = c("", "TotalFixDur (s)"),title = "Total Fixation Duration")
     ```

2. **描述性图表**
   - 箱线图展示不同条件下的数据分布
   - 直方图展示数据频率分布
   - 添加均值线辅助解读
     ```R
     RQ2_PercentDur_single <- ggplot(AOI_single_H, aes(x = AOI, y = PercentDur, fill = AOI))+
       stat_boxplot(geom = "errorbar", width = 0.15) + 
       geom_boxplot(stat = "boxplot", alpha = 0.5)
     ```

3. **组合图表**
   - 使用grid.arrange组合多个图表
     ```R
     Fixation_AOI_plot <- grid.arrange(FixDur_Video_plot,FixDur_ST_plot,FixDur_TT_plot,
                                   FixNum_video_plot,FixNum_ST_plot,FixNum_TT_plot, 
                                   nrow = 2, ncol = 3)
     ```
   - 保存高分辨率图表
     ```R
     ggsave("TotalFixation_plot.jpeg",TotalFixation, device="jpeg",dpi = 400, width = 6, height = 4)
     ```



---