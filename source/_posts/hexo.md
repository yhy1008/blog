---
title: Hexo搭建个人博客
tags:
  - hexo
  - 测试
categories: 随便写写
date: 2019-12-04 14:41:31
---
*利用hexo搭建个人博客，此时已经毕业半年才开始可能已经晚了（以前在学校时总以为搭建一个自己的博客肯定很难，结果是我想错了，所以事情一定要去尝试努力过后才有资格去否定），但我不想放弃。*

### 一、准备工作

1.npm安装（Node.js下载安装），因为Hexo需用通过npm安装，而npm需要node，只要安装好node 就会自带npm，这是（自我感觉）最简单的方式。

2.Github账号，Git下载（准备部署在Github上）

### 二、安装Hexo

**Install Hexo**

- 鼠标右键选择Git Bash Here（~~win+R打开cmd~~），执行命令

```bash
npm install -g hexo-cli
hexo init blog
cd blog
npm install
hexo server
```
- 在浏览器输 http://localhost:4000 本地预览效果,就能看到博客网站了。