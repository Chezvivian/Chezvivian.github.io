---
title:'2023-5-23 讲座录音+自动生成会议纪要的流水线作业' 
tags:
  - technical
---

今年上半年跟 Youtube 上的大佬学了一个讲座录音自动生成会议纪要的 pipeline。测试了几次，发现对10分钟之类的录音转化效果还可以，基本不会出错。但是20分钟以上，甚至1个小时的内容就几乎必报错。所以花了一天写的流程，实际上使用的场景很有限。我也一直想优化一下流程，让将来一小时、两小时的讲座也能自动输出结果。

## 初始流程

当时详细的步骤发布在这个 [Notion page](https://verbose-temple-e01.notion.site/df1617fe30d0450ca12497f7dd4bce3d) 上，现在先简要回顾一下 pipeline 的主要步骤：

1. Pipedream (自动化平台) 中新建一个流程。初始录音文献需从各个终端上传到 google drive. 
2. Trigger 2: 流程中添加从 google drive 中获取缓存文件
3. Trigger 3: 通过 ChatGPT API 转录音频文件
4. Trigger 4: 通过 ChatGPT API prompts 下达总结会议纪要的指令
  1. Query/user message
  2. Context
  3. Instructions/system message
5. Trigger 5: formatter: Node app → pass data between steps → 把之前的summary 精简成笔记
6. Trigger 6: 连接回 Notion 的 database, 设定新 Page 的内容格式

## 出现的问题

问题主要有两方面：1. 录音时间过长，转录过程中 timeout 报错，2. 转录后的文本过长， 超过单个 ChatGPT prompt 可接收的字符量。

目前第一个问题可以通过讯飞的录音笔自动转录解决，之后再测试一下讯飞 APP 能否保存1小时以上的转录内容。

第二个问题 Youtube 上的 Notion 大佬好像提出了把文本拆分为几个内容喂给 ChatGPT 的方法。待稍后试一试。
