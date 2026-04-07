# 币圈老秦的 Hexo 博客项目

## ✅ 项目已搭建完成

博客已创建在：`~/.qclaw/workspace/laoqin-blog/`

---

## 🚀 本地预览

在终端执行：
```bash
cd ~/.qclaw/workspace/laoqin-blog
npx hexo server
```
然后打开浏览器访问 **http://localhost:4000**

---

## 📝 写文章

```bash
cd ~/.qclaw/workspace/laoqin-blog
npx hexo new "文章标题"
```

文章会生成在 `source/_posts/` 目录，编辑 `.md` 文件即可。

### 文章模板：
```markdown
---
title: 你的标题
date: 2026-04-07
categories:
  - 分类名
tags:
  - 标签名
description: 文章简介
---

正文内容...
```

---

## 🌍 部署到 GitHub Pages

### 1️⃣ 初始化 Git（仅首次）
```bash
cd ~/.qclaw/workspace/laoqin-blog
git init
git add .
git commit -m "init blog"
```

### 2️⃣ 创建 GitHub 仓库
1. 打开 https://github.com/new
2. 仓库名：`laoqin-crypto.github.io`（换成你的用户名）
3. **不要**勾选 README
4. 点击 "Create repository"

### 3️⃣ 推送代码
```bash
cd ~/.qclaw/workspace/laoqin-blog
git remote add origin https://github.com/你的用户名/laoqin-crypto.github.io.git
git push -u origin main
```

### 4️⃣ 配置部署并发布
编辑 `_config.yml`，找到 `deploy` 部分：
```yaml
deploy:
  type: git
  repo: https://github.com/你的用户名/laoqin-crypto.github.io.git
  branch: main
```

然后执行：
```bash
npx hexo clean
npx hexo generate
npx hexo deploy
```

首次部署后，等待 **1-2 分钟**，访问 `https://你的用户名.github.io` 即可看到博客！

---

## 🎨 主题配置

主题配置在 `themes/butterfly/_config.yml`

常用配置：
- 社交链接（GitHub、邮箱）
- 个人简介
- 公告内容
- 颜色主题

---

## 📂 项目结构

```
laoqin-blog/
├── _config.yml          # 主配置
├── themes/
│   └── butterfly/       # 主题配置
├── source/
│   ├── _posts/         # 文章目录
│   ├── about/          # 关于页
│   ├── tags/           # 标签页
│   ├── categories/    # 分类页
│   └── img/            # 图片目录
└── public/             # 生成的静态文件
```

---

## ⚠️ 注意事项

1. **文章用 Markdown 写**，格式简单易学
2. **每次修改后**记得 `hexo clean && hexo generate && hexo deploy`
3. **图片放** `source/img/` 目录，文章中用 `/img/图片名.png` 引用
4. **以后我会帮你**写文章、部署，有什么需要随时说！

---

有问题随时问我！ 🦊