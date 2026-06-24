# 赵伟 - 个人学术主页

[![Hugo](https://img.shields.io/badge/Hugo-v0.154+-blue?logo=hugo)](https://gohugo.io/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE.md)

基于 [Hugo](https://gohugo.io/) + [HugoBlox](https://hugoblox.com/) 搭建的个人学术主页，用于展示研究方向、学术成果、项目经历等信息。

**🔗 在线访问：** [https://localhost:1313](http://localhost:1313)（本地预览）

---

## 📋 项目简介

本网站是赵伟（Wei Zhao）的个人学术主页，主要展示以下内容：

- **教育背景** — 博士、硕士、本科就读经历
- **研究方向** — 差异隐私、深度学习隐私保护、强化学习、计算机视觉
- **学术成果** — 已发表论文及学术出版物
- **项目经历** — 研究项目详细介绍
- **联系方式** — 邮箱、社交平台等联系信息

---

## 🛠 技术栈

| 组件 | 技术 |
|------|------|
| 静态网站生成器 | [Hugo](https://gohugo.io/) (v0.154+) Extended |
| 主题框架 | [HugoBlox (Wowchemy)](https://hugoblox.com/) v5.9 |
| 前端样式 | Bootstrap 5 |
| 数学公式 | MathJax 3 |
| 图标 | Academicons + Font Awesome |
| 内容格式 | Markdown + YAML |
| 语言 | 中文 (zh-Hans) |

---

## 🚀 快速开始

### 环境要求

- [Hugo Extended](https://gohugo.io/installation/) v0.112.0 或更高版本
- [Git](https://git-scm.com/)（用于 Hugo Modules）
- [Go](https://go.dev/) 1.19+（用于 Hugo Modules）

### 本地运行

```bash
# 克隆项目
git clone <your-repo-url> zhaowei
cd zhaowei

# 启动本地开发服务器
hugo server -D

# 浏览器访问 http://localhost:1313
```

### 构建部署

```bash
# 生成静态文件（输出到 public/ 目录）
hugo --minify

# 部署 public/ 目录到任意静态托管服务
```

---

## 📁 项目结构

```
zhaowei/
├── config/_default/        # 网站配置
│   ├── hugo.yaml           #   Hugo 主配置
│   ├── params.yaml         #   外观、SEO、功能参数
│   ├── languages.yaml      #   语言配置
│   ├── menus.yaml          #   导航菜单
│   └── module.yaml         #   Hugo 模块配置
├── content/                # 网站内容
│   ├── _index.md           #   首页（Landing Page）
│   ├── publication/        #   学术论文
│   ├── post/               #   研究项目/博客
│   ├── people/             #   个人信息
│   ├── contact/            #   联系方式
│   └── tour/               #   研究方向
├── assets/                 # 前端资源（CSS/JS/图片）
├── layouts/                # 自定义布局模板
├── static/                 # 静态文件
├── images/                 # 原始图片素材
├── public/                 # 构建输出（自动生成）
├── go.mod                  # Go 模块依赖
└── theme.toml              # 主题元信息
```

---

## ⚙️ 自定义配置

### 修改网站信息

编辑 [config/_default/hugo.yaml](config/_default/hugo.yaml)：

```yaml
title: 你的网站标题
baseURL: "https://yourdomain.com/"
```

### 修改外观和功能

编辑 [config/_default/params.yaml](config/_default/params.yaml)：

- `appearance.theme_day` — 日间主题（minimal / dark 等）
- `appearance.font` — 字体样式
- `marketing.seo.description` — SEO 描述
- `footer.copyright.notice` — 页脚版权信息

### 修改导航菜单

编辑 [config/_default/menus.yaml](config/_default/menus.yaml)。

### 添加学术论文

在 [content/publication/](content/publication/) 目录下创建新文件夹，包含 `index.md`，格式参考已有论文。

---

## 🚢 部署方式

本项目支持多种静态托管平台：

| 平台 | 说明 |
|------|------|
| **GitHub Pages** | 推送至 GitHub，配合 GitHub Actions 自动构建 |
| **Netlify** | 连接 Git 仓库，自动构建部署 |
| **Vercel** | 导入项目，零配置部署 |
| **Cloudflare Pages** | 连接仓库，自动构建 |
| **自有服务器** | 将 `public/` 目录部署到 Nginx/Apache |

### GitHub Pages 部署示例

在仓库设置中启用 GitHub Pages，构建命令：

```bash
hugo --minify --baseURL "https://<username>.github.io/<repo>/"
```

---

## 📝 内容编写指南

- 使用标准 Markdown 语法编写内容
- 数学公式支持 LaTeX：`$E = mc^2$` 或 `$$\int_0^\infty f(x)dx$$`
- 论文引用支持 BibTeX 格式导入
- 图片放在 `assets/media/` 或 `static/` 目录下

---

## 📄 许可证

本项目基于 [MIT 许可证](LICENSE.md) 开源。

---

## 🙏 致谢

- [Hugo](https://gohugo.io/) — 静态网站生成器
- [HugoBlox / Wowchemy](https://hugoblox.com/) — 学术网站主题框架
- [Bootstrap](https://getbootstrap.com/) — 前端 UI 框架
