# EthanLiu6 的个人博客

基于 [Hugo](https://gohugo.io) + [hugo-theme-next](https://github.com/hugo-next/hugo-theme-next) 的个人博客，通过 GitHub Actions 自动构建部署到 GitHub Pages。

## 目录结构

```
├─ content/
│  ├─ about/       关于我（单页）
│  ├─ archives/    归档页
│  └─ posts/       所有文章（统一放这里，共 100+ 篇）
├─ static/
│  ├─ imgs/        站点图片（头像、收款码等，URL 为 /imgs/…）
│  └─ pdf/         文章引用的 PDF（URL 为 /pdf/…）
├─ layouts/        自定义模板覆盖
├─ themes/         hugo-theme-next 主题
├─ archetypes/     新建文章模板
├─ hugo.yaml       站点配置
└─ POSTS_INDEX.md  分类与标签总索引（写作前必查）
```

## 写作规范

### 文件名

统一使用 `YYMMDD-简单命名.md` 格式（YY=年份后两位，MMDD=月日）：

```
2025 年 10 月 24 日 → 251024-大模型的一些知识.md
2026 年 7 月 13 日 → 260713-中文名.md
```

### 文章 front matter（YAML）

```yaml
---
aliases:            # 可选：旧链接自动跳转（迁移时自动生成，新文可留空或删掉）
  - /posts/001-旧名/
title: "文章标题"
date: 2026-07-13
draft: false
tags: ["标签1", "标签2"]
categories: ["分类1", "分类2"]
---
```

- `categories` 用于大方向归类（对应顶部菜单的「我的感悟 / 我的学习 / 我的比赛 / 我的功过」）
- `tags` 用于更细粒度的标签
- 打标签前先查 `POSTS_INDEX.md`，保持名称统一、避免再造出重复/近似标签

### 分类与标签

分类和标签的完整清单及使用次数见根目录的 `POSTS_INDEX.md`。分类页、标签页由 Hugo 自动生成：`/categories/…`、`/tags/…`。

## 本地开发

```bash
hugo server -D        # 本地预览（含草稿）
hugo server           # 本地预览（仅正式文章）
hugo                  # 构建到 docs/（publishDir）
```

## 部署

推送到 `master` 分支后，GitHub Actions 会自动构建并部署到 GitHub Pages，无需手动操作。

## 迁移说明

2026-08 重构：原来分散在 `posts/`、`think/`、`learn/`、`gongguo/` 的文章已全部合并到 `content/posts/`，统一命名。每篇迁移过的文章都在 front matter 注入了 `aliases`，旧地址（`/think/…`、`/learn/…`、`/gongguo/…`、`/posts/00X-…`）会自动跳转到新地址，外部链接不受影响。