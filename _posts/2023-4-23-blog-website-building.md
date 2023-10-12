---
title: '2023-4-23 Building my blog website on Github'
date: 2023-4-23
tags:
  - cool posts
---


# 2023-4-23 Building my blog website on Github

April 23, 2023 

## 写在前面

<aside>
⚽ 今天的部署过程大概只有半个小时。比较欣喜的是发现了上次网站各个界面没有成功publish的原因，并且编写了talks下面的一条内容。就把今天的进度标记一下，作为我个人blog网站更新的开始。

</aside>

## Tools and Basics

1. Uses the template of the https://github.com/academicpages/academicpages.github.io repository
2. Fork it, change the meta data and upload my own content

## Customization procedures

### 1. 修改 _config.yml 根文件
  
  - 更改关键信息：网站名、姓名、url (github.io后缀的网址）、repository (你自己的repository)等
  - 注意：url一定要填写准确，否则在站内其他页面的相对路径会出错。



### 2. 修改_data/文件夹下的author.yml, navigation.yml 两个文件

  - author.yml: 姓名等基本信息
  - navigation.yml: 主页指向的其他页面—相对路径。默认包括publications, talks, teaching, portfolio, blog posts, CV和guide 七个界面。可以增删。增加的话需要在根目录增加相应的文件夹和内容。



### 3. 修改_pages/文件夹下各个界面的html/md导航内容

  - 内容格式可以是html，也可以是md。


### 4. 上传各个界面文件夹下的具体内容，比如CV, talks, publications等，根据内容编写md/html文件。

  - 目前可操作的方法有(根据ChatGPT的建议）：
    1. 在Notion中编写文档，如本文档，再export为markdown & csv文件，选取md文件上传。
    2. 直接在编辑器中编写md文档。有需要上传图片的地方，写好引用位置，再把图片单独上传到images/或者相应的文件夹中。

# 2023-10-12 解决blog中文无法显示的问题

其实4月23日已经写下第一篇blog，但是网站上一直无法显示（blog栏目下为空白）。效率优先，我就先把blog部分隐藏，网站上线。

今天突然想更新一些阅读感想，就继续来看这个问题。根结似乎出在 _data/ui_text.yml 中，默认显示语言中并未配置中文。试一试找解决方案。
