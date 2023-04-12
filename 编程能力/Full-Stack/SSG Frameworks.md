---
title: SSG Frameworks
tags: Coding   
started: 2023-03-08 Wed
due: 
modified: 2023-03-08 Wed
status: 
---
## What
- Static Site Generators (SSG)
- Used to create extremely fast and optimized websites.
- SEO, performance, flexibility, security
- Can still be dynamic and fetch data from an API or headless CMS
- All data fetching happens before build time
## Requirement
#### 1. Client Side
- Markdown > HTML
#### 2. Client Side / CMS
- Markdown Editing Experience
## SSG-General
#### 1. Astro
![[Pasted image 20230308175352.png]]
- Top level `await`
## SSG-React
#### 1. Gatsby
![[Pasted image 20230308175443.png]]
## SSG-Vue
#### 1. VuePress2 
- [VuePress2](https://v2.vuepress.vuejs.org/) 
	- What?
		- A VuePress site is in fact a single-page application (SPA) powered by [Vue](https://vuejs.org/) and [Vue Router](https://router.vuejs.org/).
		- Routes are generated according to the relative path of your markdown files. Each Markdown file is compiled into HTML with [markdown-it](https://github.com/markdown-it/markdown-it) and then processed as the template of a Vue component. This allows you to directly use Vue inside your Markdown files and is great when you need to embed dynamic content.
		- During development, we start a normal dev-server, and serve the VuePress site as a normal SPA. If you’ve used Vue before, you will notice the familiar development experience when you are writing and developing with VuePress.
		- During build, we create a server-rendered version of the VuePress site and render the corresponding HTML by virtually visiting each route. This approach is inspired by [Nuxt](https://nuxtjs.org/)'s `nuxt generate` command and other projects like [Gatsby](https://www.gatsbyjs.org/)
	- Why not ...?
		- Nuxt (Designed for building applications, while VuePress is more **lightweight** and focused on **content-centric static sites**.)
		- Vitepress (More opinionated and less **configurable**. It does not support plugins.)
		- Gitbook (Its **development reload performance** is intolerable with a large amount of files. The default **theme** also has a pretty limiting navigation structure, and the theming system is, again, not Vue based. The **team behind** GitBook is also more focused on turning it into a commercial product rather than an open-source tool.)
		- Hexo (**Theming** system is static and string-based - we want to take advantage of Vue for both the **layout and the interactivity**. Also, Hexo's **Markdown rendering** isn't the most flexible to configure)
		- Docsify / Docute (Both fully runtime-driven and therefore not **SEO**-friendly. If you don't care for SEO and don't want to mess with **installing dependencies**, these are still great choices.)

#### 2. Gridsome
![[Pasted image 20230308175509.png]]
## SSG-Node
#### 1. Ghost
- [Ghost 博客搭建日记](https://halfrost.com/ghost_build/)
#### 2. Hexo
![[Pasted image 20230308181728.png]]
## SSG-Other
#### 1. Jekyll
![[Pasted image 20230308175525.png]]
#### 2. Hugo
![[Pasted image 20230308181708.png]]
#### 3. Pelican
![[Pasted image 20230308181745.png]]
#### 4. Github
- GitHub Pages (Jekyll- 访问速度慢的实在不能忍 > 自购阿里云服务器 > Ghost)
## Inspiration
#### 1. Books (Publication)/ Documentation
- 文档是基于 [VuePress2](https://v2.vuepress.vuejs.org/) 构建，图使用 [Fabric.js](http://fabricjs.com/) 绘制，通过 Github Actions 自动部署, 大家可以在右上角访问 Github 地址，或者访问每个页面下方的修改链接，随时通过 PR 的方式共建这个知识图谱， Java，Python 等岗位的知识图谱正在制作中，欢迎一起共建一个最好的计算机知识图谱
- 路线图的数据格式大家可以参考 [docs/index.md](https://github.com/shengxinjing/it-roadmap/blob/main/docs/index.md)
- 这个网站会一直以静态的形式存在，不需要登录，不需要关注公众号，源码和文稿全部在 Github，欢迎大家一起来提 PR 共建
- 文件夹 docs 下面就是全部的文档，roadmap 组件负责渲染路线图，动态渲染
- ![[Portfolio-个人主页 2023-03-11 15.12.05.excalidraw]]
- Interactive Mindmap
- Link to **Book Site** ([Books](https://books.halfrost.com/))
	- Edit this page
	- Last modified
	- Github Comment