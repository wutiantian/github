<!-- TOC -->

- [官方手册](#官方手册)
  - [官方说明手册](#官方说明手册)
  - [官方高级搜索入口](#官方高级搜索入口)
- [开源项目的组成部分](#开源项目的组成部分)
- [筛选条件](#筛选条件)

<!-- /TOC -->

# 官方手册

## 官方说明手册

摘自： ```https://docs.github.com/cn/free-pro-team@latest/github/searching-for-information-on-github/searching-for-repositories```

按仓库名称、说明或自述文件内容搜索
基于仓库的内容搜索
在用户或组织的仓库内搜索
按仓库大小搜索
按关注者数量搜索
按复刻数量搜索
按星号数量搜索
按仓库创建或上次更新时间搜索
按语言搜索
按主题搜索
按主题数量搜索
按许可搜索
按公共或私有仓库搜索
基于仓库是否为镜像搜索
基于仓库是否已存档搜索
基于具有 good first issue 或 help wanted 标签的议题数量搜索
延伸阅读

## 官方高级搜索入口

>https://github.com/search/advanced



# 开源项目的组成部分

在讲清楚之前呢，我们先来了解一下一个开源项目有哪些组成部分：

    name: 项目名
    description: 项目的简要描述
    项目的源码
    README.md: 项目的详细情况的介绍

那么除了这些要素之外，项目本身的star数和fork数，也是评判一个开源项目是否火热的标准，这同时也是一个很重要的搜索标准。另外我们也要注意观察这个项目的最近更新日期，因为项目越活跃，那么它的更新日期也更加频繁。

以上要素就是我们在进行搜索的时候要注意的一些关键点。




# 筛选条件

想要进行精准搜索，无非就是增加筛选条件。

    in:name xxx // 按照项目名搜索
    in:readme xxx // 按照README搜索
    in:description xxx // 按照description搜索

那么在这里面呢，我们又可以增加筛选条件

    stars:>xxx // stars数大于xxx
    forks:>3000 // forks数大于xxx
    language:xxx // 编程语言是xxx
    pushed:>YYYY-MM-DD // 最后更新时间大于YYYY-MM-DD



搜索项目名里面包含React的项目:

in:name React


精确到项目的star数大于5000+：


in:name React stars:>5000

按照fork的数量来进行搜索:

in:name React stars:>5000 forks:>3000

搜索README.md里面包含React的项目:

 in:readme React

 再限制一下它的star数和fork数：

 in:readme React stars:>3000 forks:>3000

 搜索项目描述(description)里面包含微服务的项目:

 in:description 微服务

 language:python的意思是我们把语言限制为python

 in:description 微服务 language:python

我们把项目的最后更新时间限制到2020-01-01

in:description 微服务 language:python pushed:>2020-01-01

