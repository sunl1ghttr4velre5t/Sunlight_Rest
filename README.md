# Sunlight_Rest

> You can't re everything. So I stay.

Redem 的个人博客 —— 逆向工程的摸索、旅途随笔，和一些随手写下的小诗。

线上地址：<https://sunl1ghttr4velre5t.github.io/Sunlight_Rest/>

## 写一篇新文章

在 `_posts/` 下新建文件，**文件名必须是 `YYYY-MM-DD-英文短标题.md`**，例如
`2026-10-01-My-First-Writeup.md`。这个文件名决定了文章的网址。

文件开头是 front matter（三横线之间的部分），后面用 Markdown 写正文：

```markdown
---
layout: post
title: "文章标题"
date: 2026-10-01 12:00:00 +0800
categories: 随笔
description: 首页列表里显示的一句话摘要（可省略）
---

正文从这里开始。

普通换行会直接生效，一段话之间空一行即可。
```

保存并推送到 GitHub，网站会自动重新构建，**首页和归档页的列表会自动更新**，不用手动改任何链接。

## 想改样式 / 文字

| 想改什么 | 改哪里 |
| --- | --- |
| 站点名、副标题、描述、导航 | `_config.yml` |
| 颜文字、间距、圆角等所有外观 | `assets/css/style.css`（纯手写 CSS，顶部是设计变量） |
| 页面骨架 | `_layouts/*.html` |
| 顶栏 / 页脚 / `<head>` | `_includes/*.html` |

样式全部集中在 `assets/css/style.css` 的 `:root` 变量里，改一处即可全站生效，
并且已内置深色模式（跟随系统设置自动切换）。

## 目录结构

```
_config.yml              站点配置
index.md                 首页
archive.md               归档页
_posts/                  文章（Markdown）
_layouts/                页面模板
_includes/               可复用片段（顶栏、页脚、head）
assets/css/style.css     全站样式
assets/images/           图片
assets/pdf/              可下载的 PDF
```
