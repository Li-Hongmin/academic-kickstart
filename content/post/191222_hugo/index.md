---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "【学习笔记】用Hugo建站来写个人博客 Day2"
subtitle: "把Hugo的网站部署到Github pages"
summary: ""
authors: []
tags: [hugo, github pages, personal website]
categories: []
date: 2019-12-22T23:53:20+09:00
lastmod: 2019-12-22T23:53:20+09:00
featured: false
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

**上次我们已经做个一个网站在本地了，这次要把它部署到Github pages上。**

**本文主要参考[hugo官方文档](https://gohugo.io/hosting-and-deployment/hosting-on-github/),需要github和本地两别操作。**

# 部署前的准备
首先要确认三点：
1. 确认本地有无[git](https://git-scm.com/downloads):
```terminal
git --version
# git version 2.21.0 (Apple Git-122.2)
```

2. 确认[GitHub](https://github.com/)账号有无，可以免费申请一个。

3. 已经有一个可以发布的Hugo网站

# 两种GitHub Pages

1. User/Organization Pages (https://<USERNAME|ORGANIZATION>.github.io/)
2. Project Pages (https://<USERNAME|ORGANIZATION>.github.io/<PROJECT>/)

# 部署设置

1. 在github创建新的pages repository，如果是第一种就把<USERNAME|ORGANIZATION>换成你的用户名或者组织名，则输入如下图：
{{< figure src="creatpages.png" title="我因为已经有同名的repository了，所以不可以创建。" lightbox="true" >}}

2. 再用同样的方法在github创建新的repository用来放hugo的文件，以下用```<YOUR-PROJECT>```代替这个repository的名字

3. 本地git clone，把```<YOUR-PROJECT-URL>```换成网页url地址，在合适的目录下执行命令:
```git clone <YOUR-PROJECT-URL> && cd <YOUR-PROJECT>```

4. 复制粘贴之前hugo的文件到clone的目录下面。用```hugo server```来检查下正不正常，浏览器打开[http://localhost:1313](http://localhost:1313)。

5. 测试过后，用```rm -rf public/```来移除所有public下的文件。

6. 创建一个submodule：```git submodule add -b master git@github.com:<USERNAME>/<USERNAME>.github.io.git public```

这个submodule就会同步到```<USERNAME>/<USERNAME>.github.io```，而整个本地目录会同步到```<YOUR-PROJECT>```这里。

# 部署网站

## 生成网站并部署

```terminal
hugo
cd public
git add .
git commit -m "Build website"
git push origin master
cd ..
```
这样应就可以了，浏览器打开```<USERNAME>.github.io```就可以看到了。

## 自动部署脚本

可以创建一个deploy.sh文件，好像[这样](https://github.com/Li-Hongmin/academic-kickstart/blob/master/deploy.sh).

然后记得```chmod +x deploy.sh```赋予权限。

只要运行 ```./deploy.sh "Your optional commit message"```就可以提交更改了。

## 总结

流水线作业，总是不够详细。

另外本网站的制作是根据academic模版，依照其[官网](https://sourcethemes.com/academic/zh/docs/deployment/)而部署，也很简单。