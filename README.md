# 赵伟 - 个人学术主页

[![Hugo](https://img.shields.io/badge/Hugo-v0.154+-blue?logo=hugo)](https://gohugo.io/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE.md)
[![GitHub Pages](https://img.shields.io/badge/GitHub-Pages-black?logo=github)](https://zhaowei-zwgit.github.io/)

基于 [Hugo](https://gohugo.io/) + [HugoBlox](https://hugoblox.com/) 构建的个人学术主页，展示研究方向、学术成果、教育背景等信息。

🔗 **在线访问：** [https://zhaowei-zwgit.github.io](https://zhaowei-zwgit.github.io)

---

## 快速开始

### 环境要求

- [Hugo Extended](https://gohugo.io/installation/) v0.112.0+
- [Git](https://git-scm.com/)
- [Go](https://go.dev/) 1.19+

### 本地运行

```bash
git clone https://github.com/zhaowei-zwgit/zhaowei-zwgit.github.io.git
cd zhaowei-zwgit.github.io
hugo server -D
```

访问 `http://localhost:1313` 预览。

### 构建部署

```bash
hugo --minify
```

生成的静态文件在 `public/` 目录，部署到任意静态托管平台即可。

---

## 项目结构

```
├── config/_default/     # 网站配置（hugo.yaml、params.yaml、menus.yaml 等）
├── content/             # 网站内容
│   ├── _index.md        #   首页
│   ├── publication/     #   学术论文
│   ├── post/            #   研究项目
│   ├── people/          #   个人信息
│   ├── contact/         #   联系方式
│   └── tour/            #   研究方向
├── assets/              # 前端资源（SCSS、图片）
├── layouts/             # 自定义布局模板
└── .github/workflows/   # GitHub Actions 自动部署
```

---

## 自定义

| 配置文件 | 用途 |
|---------|------|
| [hugo.yaml](config/_default/hugo.yaml) | 网站标题、URL、语言等基础配置 |
| [params.yaml](config/_default/params.yaml) | 主题、外观、SEO、功能参数 |
| [menus.yaml](config/_default/menus.yaml) | 导航菜单 |
| [languages.yaml](config/_default/languages.yaml) | 语言设置 |

添加论文：在 `content/publication/` 下新建文件夹，参考已有论文格式编写 `index.md`。

---

## 技术栈

- **生成器：** [Hugo](https://gohugo.io/) Extended
- **主题：** [HugoBlox](https://hugoblox.com/) (Wowchemy)
- **样式：** Bootstrap 5
- **公式：** MathJax 3
- **图标：** Academicons + Font Awesome

---

## 部署

项目通过 GitHub Actions 自动部署到 GitHub Pages。推送到 `main` 分支即可触发自动构建。

也支持 Netlify、Vercel、Cloudflare Pages 等平台。

---

## 许可证

[MIT](LICENSE.md)
