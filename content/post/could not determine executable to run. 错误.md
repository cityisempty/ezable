---
title: could not determine executable to run. 错误
source: 
author:
  - Lice
published: 2025-03-08
created: 2025-03-09
description: ""
tags:
  - clippings
  - 错误提示
date: 2025-03-09
slug: 14:41
share: true
canonicalURL: ""
series: 系列
lastmod: 
lang: cn
cover:
  image: ""
dir: post
categories:
  - 错误记录
weight: 1
---
## 什么时候发生的？

尝试将 TailwindCSS 引入 React 时会发生这种情况。  
使用的命令和实际错误屏幕如下：

```
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```
![错误](https://storage.googleapis.com/zenn-user-upload/8746195eca4b-20250201.png)

TailwindCSS 的最新版本几天前刚刚发布`V4.0`，安装方法有所改变。

[开始使用 Tailwind CSS](https://zenn.dev/o0rororo0o/articles/%5B%E3%83%AA%E3%83%B3%E3%82%AF%E3%81%AEURL%5D\(https://tailwindcss.com/docs/installation/using-vite\))

## [](https://zenn.dev/o0rororo0o/articles/003183a9a9d76a#%E8%A7%A3%E6%B1%BA%E6%B3%95)解决方案

使用旧版本的 tailwind, 
```
$ npm install -D tailwindcss@3 postcss autoprefixer
```

`Vite`要在使用 TailwindCSS 的项目中安装它，`V4.0`请使用以下命令。

```
npm install tailwindcss @tailwindcss/vite
```

总结就是v4 安装方法变了, 可以使用v3

