---
title: 博客添加tags及categories
date: 2019-12-05 17:31:17
tags: hexo
categories: 随便写写
---
- ### 创建分类和标签文件夹

```bash
hexo new page categories
hexo new page tags
```
<!--more-->

**找到各自文件夹下index.md这个文件，打开后并修改**

```
title: categories
date: 2019-12-04 15:26:59
type: categories
---
title: tags
date: 2019-12-04 15:10:52
type: tags
```

- ### 配置菜单，「分类」、「标签」这些菜单

```
menu:
  home: /
  archives: /archives
  tags: /tags
  categories: /categories
```

- ### 新建一遍文章添加分类和标签

`hexo new "文件名"`

**在文件内添加**
```
title: Hexo搭建个人博客
date: 2019-12-04 14:41:31
tags: [hexo,测试]
categories: 随便写写
```

- ### Markdown基本语法

进入[Markdown](https://www.jianshu.com/p/191d1e21f7ed)