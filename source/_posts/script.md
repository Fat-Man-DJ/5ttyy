---
title: 全自动部署Hexo+Vercel,本地写博客
date: 2020/7/1
categories: Hexo
tags:
  - Hexo
  - Git
---

一天,我在洗澡的时候,想

```
要是我能不忍Github的垃圾编辑器??
```

然后,这个脚本就诞生了

其实挺简单的,就这几句话:

```shell
git add *
git commit -m "creat a blog"
git push -f
```


用法:
git clone我的博客
删除.git文件夹
按照网上教程去初始化并添加repo

让后运行autoDeploy即可

而且还需要GIT

但不过还是挺好用的

```shell
Tips:如果对配置文件有改动,要在本地改然后push
不然会造成不同步问题
别问我怎么知道的
```
