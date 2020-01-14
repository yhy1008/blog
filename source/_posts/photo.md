---
title: Hexo 在博文中插入图片
tags:
  - photo
categories:
  - 随便写写
date: 2019-12-10 17:39:00
---

![插入本地图片](photo/20191210.jpg)
<!--more-->

- 插入本地图片需要修改主题_config.yml配置文件post_asset_folder项为true

- 使用插件达到插入本地图片，在根目录输入如下命令安装：

`npm install hexo-asset-image --save`

上面的命令可能会有问题，然后执行下面的命令：

`npm install https://github.com/CodeFalling/hexo-asset-image --save`

之后new 一篇博客时/source/_posts文件夹内除了xxxx.md文件还有一个同名的文件夹，把图片放到里面即可，最后在xxxx.md中想引入图片时，先把图片复制到xxxx这个文件夹中，最后只需要在xxxx.md中按照markdown的格式引入图片：
![你想输入的替代文字]（xxxx/图片名.jpg）就可以了。