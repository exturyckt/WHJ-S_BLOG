# Hexo 博客仓库

本仓库包含了我的个人 Hexo 博客的源码和配置文件，其中包括主题自定义和额外功能，提供了一个完整的博客内容。

[博客链接](https://wtmdyszl.website)
[更为详细的搭建教程](https://blog.cuijiacai.com/blog-building/)
## 功能特性

- **Hexo 框架**：一个快速、简单且功能强大的静态站点生成器。
- **自定义主题**：使用 [Butterfly](https://github.com/jerryc127/hexo-theme-butterfly) 并进行了个性化配置。
- **社交媒体集成**：包含 GitHub、B站等社交链接。
- **Markdown 支持**：所有文章使用 Markdown 编写，简单高效。
- **音乐页面**：推荐音乐的独立页面。
- **标签和分类**：组织内容，方便导航。

## 快速开始

### 环境要求

在开始之前，请确保你的电脑上已安装以下工具：

- [Node.js](https://nodejs.org/)（建议使用 v16 或更高版本）
- [Git](https://git-scm.com/)
- [Hexo CLI](https://hexo.io/zh-cn/docs/)：通过 npm 安装：
  ```bash
  npm install -g hexo-cli
  ```

### 安装

1. 克隆此仓库：
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   ```
2. 进入项目目录：
   ```bash
   cd your-repo-name
   ```
3. 安装依赖：
   ```bash
   npm install
   ```

### 本地运行博客

1. 启动 Hexo 本地开发服务器：
   ```bash
   hexo server
   ```
2. 打开浏览器并访问：[http://localhost:4000](http://localhost:4000)

### 部署博客

1. 生成静态文件：
   ```bash
   hexo generate
   ```
2. 部署到 GitHub Pages：
   ```bash
   hexo deploy
   ```

   请确保你的 `_config.yml` 中的 `deploy` 部分已正确配置。

## 目录结构

```plaintext
.
├── source/                 # 博客文章、页面和静态资源
│   ├── _posts/            # 文章的 Markdown 文件
│   ├── music/             # 音乐页面的文件
│   └── ...
├── themes/                # 主题文件
├── _config.yml            # Hexo 配置文件
├── package.json           # npm 依赖和脚本
└── ...
```

## 自定义

### 社交媒体链接

在主题的 `_config.yml` 文件中更新 `social` 部分来添加或修改社交媒体链接：

```yaml
social:
  fab fa-github: https://github.com/your-username
  fas fa-envelope: mailto:your-email@example.com
  fab fa-bilibili: https://space.bilibili.com/your-id
```

### 音乐页面

将你的音乐文件（如 `.mp3`）添加到 `source/music` 目录，并在页面中列出对应的歌曲。

### 标签和分类

Hexo 会根据文章的元数据自动生成标签和分类页面。可以在 Markdown 文件中使用以下格式：

```markdown
---
title: 文章标题
date: 2025-01-13 12:00:00
tags:
  - 标签1
  - 标签2
categories:
  - 分类1
---
```

## 常见问题

### 常见问题解答

- **主题未正确应用**：确保已正确安装主题并在 `_config.yml` 中设置。
- **部署错误**：检查 `deploy` 配置和 SSH 密钥是否正确。

### 常用命令

- `hexo clean`：清除缓存和生成的文件。
- `hexo generate`：生成静态文件。
- `hexo deploy`：部署网站。
- `hexo server`：运行本地开发服务器。

---

祝你博客写作愉快！