

<p align="center">
    <img src="release/img/logo.jpg">
</p>

## Languange

[English](README.md) | 中文



## What

**ZenHo** 是一个极简风格的  [Hugo](https://gohugo.io/) 主题

> All good things come to thos who wait.



![screenshot](images/screenshot.png)

### Features

- [ ] Google 统计
- [ ] disqus 评论插件
- [x] Baidu 统计
- [x] 文章目录
- [x] utteranc 评论插件
- [x] Github 项目卡片展示


## How to use

步骤一：

​	如果你是第一次了解到 [Hugo](https://gohugo.io/) 的话，你需要先看一下官方的[入门教程](https://gohugo.io/getting-started/quick-start/)

步骤二：

​	你可能需要用 `hugo-zenHo/archetypes/default.md` 替换 Hugo 默认的 `archetypes/default.md` 文件

步骤三：

​	如果你要自定义 about 页面，需要创建  `content/about/_index.md` 文件， 然后以 markdown 格式书写内容即可 

步骤四：

​	复制 [Configuration Override](##Configuration Override) 下的内容到你的 config.toml，为了更好的代码高亮展示，建议设置主题为 xcode

```toml	
[markup]
  [markup.highlight]
    style = "xcode"
```

具体的实例可以参考 **exampleSite** 目录

## Github project card

ZenHo 使用 [github-readme-stats](https://github.com/anuraghazra/github-readme-stats) 和 shortCode 实现了 Github 项目展示。

![github-project-card](img/github-project.png)

你可以使用以下代码在你的文章中以卡片的形式展示 Github 项目

```html
{{< github-project username="your github user name" repo="your github project name" >}}
```

比如

```html
{{< github-project username="vran-dev" repo="hugo-zenHo" >}}
```


## Configuration Override

You can copy some item to your `config.toml` .

```toml
baseURL = "http://localhost:1313/"
languageCode = "en-us"
title = "ZenHo"
paginate = 6

[params]
    enableSummary = true
    useDescriptionReplaceSummary = true
    enableToc = false

    author  = "vran"
    bio = "All good things come to thos who wait."

    # baidu analytics
    enableBaiduAnalytics = false
    baiduAnalyticsToken = ""

    googleSiteVerificationToken = ""

    # social page url
    github = "#"
    twitter = "#"
    facebook = "#"
    email = ""

    # utteranc comment
    enableUtteranc = false
    [params.utteranc]
        repo="username/github-page-repository"
        theme="github-light"
        crossorigin="anonymous"
        issueTerm="pathname"
        label="Comment"

[markup]
  [markup.highlight]
    style = "xcode"
  [markup.tableOfContents]
    endLevel = 2
    ordered = false
    startLevel = 2
```



## Screenshots

- Home

  ![](release/img/home.png)



- post

  ![](release/img/post.png)

  

  ![](release/img/content-2.jpg)





- Archive

  ![](release/img/archive.jpg)

- tags

  ![](release/img/tags.jpg)



- About

  ![](release/img/about.png)

