---
title: Hexo最简入门
date: 2023-04-18 17:49:59
categories: 
- Technology
tags: 
- Hexo
- Quick start
---

# Hexo快速入门
[Hexo官方文档](https://hexo.io/zh-cn/docs)

## 安装基本环境
- Node.js

## 下载Hexo
- Hexo本体
```powershell
npm install -g hexo-cli --registry=http://registry.npmmirror.com
```

- 渲染器
```powershell
npm install --save hexo-renderer-less hexo-renderer-ejs --registry=http://registry.npmmirror.com
```

## 主题
- async  
https://async-docs.imalun.com
```powershell
npm i hexo-theme-async@latest
```

## 初始化Hexo并部署到Github pages
- 创建一个github仓库，命名为username.github.io
- 初始化仓库
- 进入git上级目录，运行
```powershell 
npx hexo init username.github.io
```
- 运行
```powershell 
cd username.github.io
npm install
```
- 更详细信息，参见https://hexo.io/zh-cn/docs/setup
- github部署信息，参见https://hexo.io/zh-cn/docs/github-pages