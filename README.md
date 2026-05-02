# 伤寒论研习社

基于 Jekyll 的简约中医伤寒论博客。

## 快速部署到 Gitee Pages

### 方法一：Gitee  Pages 自动部署（推荐）

1. 将此仓库推送到 Gitee
2. 进入仓库 → 服务 → Gitee Pages
3. 选择 `master` 分支，点击部署

### 方法二：本地预览

```bash
# 安装 Ruby 和 Jekyll
gem install jekyll bundler

# 安装依赖
bundle install

# 本地预览
bundle exec jekyll serve
```

访问 http://localhost:4000 查看。

## 博客结构

```
├── _config.yml        # 配置文件
├── _layouts/          # 页面模板
├── _includes/        # 可复用组件
├── _posts/            # 文章目录
├── _pages/            # 页面目录
├── assets/css/        # 样式文件
└── index.html          # 首页
```

## 添加新文章

在 `_posts` 目录下创建 Markdown 文件，文件名格式：

```
YYYY-MM-DD-文章标题.md
```

Front Matter 示例：

```yaml
---
layout: post
title: 文章标题
date: 2026-05-02
categories: 分类名称
---
```

## 使用 Gitee SSH 推送

```bash
# 添加远程仓库（SSH）
git remote add origin git@gitee.com:me888888/blog.git

# 推送代码
git push -u origin master
```

---

传承中医经典，弘扬古圣智慧。
