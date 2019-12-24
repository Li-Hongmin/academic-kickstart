---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "【学习笔记】用Hugo建站来写个人博客 Day1"
subtitle: "Hugo的安装和简单使用"
summary: ""
authors: []
tags: [hugo,blog,建站，博客]
categories: []
date: 2019-12-22T23:38:25+09:00
lastmod: 2019-12-22T23:38:25+09:00
featured: true
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: [hugo_website]
---
**建站一直是一个很复杂的工程，不过总有捷径。本文介绍一种快速建立静态网站的工具hugo。hugo是基于go语言新兴静态网站生成工具，非常快速轻便。我们只需要用markdown来写博客直接生成网页，可以让我们专注于内容。另外有超多主题可供选择，换个装潢模版也很容易。**

# 缘起

我目前在读Ph.D平时读论文时会做一些笔记，一直想把这些笔记整理分享出来。
我于是开始尝试使用个人博客来记录学习过程整理思路，之后还能做一些页面展示研究成果。

通过一番考察我选择先用[Hugo](gohugo.io)建立一个网站。
详细Hugo是什么请读者自行了解，我理解就是go语言写的快捷建站工具，并且只要用markdown语言就可以写页面了。
同时在过程中把自己的心得分享出来供后来者参考。

# 安装和一键建站

这里我主要参考官网的[Quick Start](https://gohugo.io/getting-started/quick-start/)。

1. 安装 Hugo
我的环境时macOS，使用Homebrew安装：

```terminal
brew install hugo
hugo version
```
最后得到这样的信息：Hugo Static Site Generator v0.61.0/extended darwin/amd64 BuildDate: unknown。


另外说Homebrew是一个非常好的软件管理软件，一行代码就安装好了，如果还没有试过的人一定要尝试一下。

如果是Windows或linux用户的话参考[这里](https://gohugo.io/getting-started/installing)进行安装。


2. 一键建站

在terminal或命令行里找个合适的文件路径，执行以下命令。

```terminal
hugo new site yourFolderName
```

这时Hugo会生成一个网站模版。命令中_yourFolderName_就是文件夹名，可以随便起。

3. 添加主题

主题是Hugo的一大优势，海量主题任你选。这里是[主题库](https://themes.gohugo.io/)。

我们这里就用官方教程里的Ananke。
```terminal
cd quickstart

# Download the theme
git init
git submodule add https://github.com/budparr/gohugo-theme-ananke.git themes/ananke
# Note for non-git users:
#   - If you do not have git installed, you can download the archive of the latest
#     version of this theme from:
#       https://github.com/budparr/gohugo-theme-ananke/archive/master.zip
#   - Extract that .zip file to get a "gohugo-theme-ananke-master" directory.
#   - Rename that directory to "ananke", and move it into the "themes/" directory.
# End of note for non-git users.

# Edit your config.toml configuration file
# and add the Ananke theme.
echo 'theme = "ananke"' >> config.toml
```

4. 添加页面

生成第一个页面。

```terminal
hugo new posts/my-first-post.md
```

第一个页面看起来像这样：
```
---
title: "My First Post"
date: 2019-03-26T08:47:11+01:00
draft: true
---
```

可以用你喜欢的IDE来写markdown文件，直接就可以生成网站了。

5. 运行Hugo服务器

终于到来一键生成网站的时候了，虽然这里的一键是一行命令。
```terminal
hugo server -D
```

最后提示
```
Web Server is available at http://localhost:1313/ (bind address 127.0.0.1)
Press Ctrl+C to stop
```

浏览器打开[http://localhost:1313/](http://localhost:1313/)看看是不是成功了。

看上去就像是[这样子](https://li-hongmin.github.io/blog/)。

# 总结

简单易学，一行命令完事。

建站大坑，容我慢慢来填。