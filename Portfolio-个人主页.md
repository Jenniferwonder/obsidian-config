---
title: Portfolio-个人主页
tags: Projects/React-Project   
started: 2023-02-16 Thu
due: 
modified: 2023-03-13 Mon
status: Doing
---
## Documentation
- [[Project Plan and Research - Portfolio]]
- [[Architecture and System Design - Portfolio]]
## Task Backlog
#### 1. Projects Pool
- [[Front-End Tech Stack]]
#### 2. Purpose and Competitive analysis
- Value
- Interest
- Strength
- **Content**
#### 3. Requirement Table 
- Community Interaction (Q&A) > **Premium Content** (Pay/ Subscribe to unlock > Password)
	- **Note > Book/ Knowledge Base** Website (Why not Yuque?)
		- Authorization 
			- Read only (Ban Content Copying)
		- Free Access 
- Share; Comment; 
- Edit
- Write and Post 
- Build a **Blog** Website
- Build a **Portfolio** Website > Blog; Projects (Github); Contact
#### 4. Inspiration and Design > Wireframe
- UI/UX
- Figma; PS
#### 5. Function Module Diagram > [[UML]] (Flow Chart/ Mindmap)
- Function (CRUD)
#### 6. Tech Architecture Diagram
- SPA/ ~~MPA~~?
#### 7. Tech Choices (Why & Why not) > Demo
- Meet UI requirement (Slice SVG to HTML) - 切图
- Front-end Framework
- [[SSG Frameworks]]
- UI Framework/ Libraries
- Back-end Framework
	- User Analytics (Visitor; Comments)
	- Tags
	- Recommend/ Related
- Database/ Data Store
	- Picture/ Music/ Video
	- Markdown > HTML
	- User
	- Post
	- Author
- Testing
- Deploy
	- CI/CD
	- Server
	- DNS
	- CDN
	- 备案
#### 8. Resources

## Purpose
### Why do I want to build a personal portfolio/ blog website?
- Enhance/ Apply the **Front-end Tech** skills I've learned about React, JS, HTML, CSS
- ⭐~~Demo~~ > ~~Full-Stack App~~ > Use GitHub **repo** and **issues** to sync/push my `.md` notes to a website (My personal website)  
- **Showcase** my <u>work and skills and blogs</u>
- Understand and master the **Front-End skills** needed to build a portfolio website 
- Benefit me and people alike
### What kind of portfolio website do I need/want to build?
- A Portfolio Website
- Production-ready project - Static and server-rendered app?
- Blog Site
	- [Halfrost's Field | 冰霜之地](https://halfrost.com/)
- Portfolio Website 
	- [Dezhi Yu](https://halfrost.me/)
	- Home (About)- SPA; 
	- Accomplishments (Certification)
	- Projects/ ->Rich Content/.md Format 
- Books
	- [Books](https://books.halfrost.com/)
- Share Talk/ Speech PPT 
	- [halfrost (@halfrost) on Speaker Deck](https://speakerdeck.com/halfrost/)
## Design 
### Inspiration
#### 1. UI Function and Feature
- **Photo/ Image**/ Logo/ Font editing (Resizing, format from jpeg to png, compressing, reshaping, changing/ removing background, anime, placeholder) 
- [[Photo Editing]]
#### 2. Inspirations
##### 2.1. Reference
- [Dezhi Yu](https://halfrost.me/)
- [大圣前端进阶指南 | 解决前端进阶的难点](https://shengxinjing.cn/)
- [coderZ-首页](https://coderzblog.cn/)
- Vue: [cdn.jsdelivr.net 凉了引发的一系列风波RBlog](https://raxcl.cn/blog/6)
- Vue: [使用 GitHub + jsDelivr + PicGo + Typora 搭建图床 - Naccl's Blog](https://naccl.top/blog/11)
- ✅[Josh Collinsworth | Blog](https://joshcollinsworth.com/blog)
- ✅SSR Fetched Blog Page: [Alicia's Notes 🚀 — Thankful to be here 🌍](https://notes.aliciasykes.com/)
- ✅With Nice CV and Blog Page: [Alicia Sykes](https://aliciasykes.com/)
- ✅Portfolio with Blogs: [学习随笔 - 以平凡开始，以平凡结束](https://www.vipyubai.top/)
- ✅Portfolio with Blogs: [GitHub - jakeherp/portfolio: My personal portfolio website, proudly built with Next.js, TypeScript and Tailwind](https://github.com/jakeherp/portfolio)
	- ❗[[Dependency Installation Error]] 
- Minimal Portfolio: [GitHub - ForrestKnight/minimal-portfolio: A developer portfolio built for a video tutorial here: https://www.youtube.com/watch?v=b0pkpcD8Ms4](https://github.com/ForrestKnight/minimal-portfolio)
- [GitHub - tbakerx/react-resume-template: A personal resume website template built with React.js, Typescript, Next.js, and styled with Tailwind css](https://github.com/tbakerx/react-resume-template)
- Reveal and animation for picture: [GitHub - 1hanzla100/developer-portfolio: Software Developer Portfolio Template built with react.js and next.js bootstrap that helps you showcase your work and skills as a software developer.](https://github.com/1hanzla100/developer-portfolio)
- >~~[Troopl](https://troopl.com) | Build and publish a free portfolio in minutes. |~~  
- [GitHub - emmabostian/developer-portfolios: A list of developer portfolios for your inspiration](https://github.com/emmabostian/developer-portfolios)
##### 2.2. Similar projects/ personal brand and marketing site.
- [[TechBlog-双语技术博客]]
- [[TechBlog 样式灵感]]
- [[01-前后端初始化与工具安装]]
- [[01-弹性盒布局方法总结：Medium 主页]]
- [[02-数据请求与预览卡片渲染]]
- [[03-预加载与富文本内容展示]]
- [[04-如何实现评论功能？]]
### Wireframe
## How to Build
### Tech Choices (Static Site Generator)
- GitHub Pages (Jekyll- 访问速度慢的实在不能忍 > 自购阿里云服务器 > Ghost)
- [Ghost 博客搭建日记](https://halfrost.com/ghost_build/)
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
- Gatsby
### Function Module Diagram ([[UML]])
#### 1. Home (About)
- Navbar(......)
- Photo; 
- Contact; 
- Summary (Education; Interest;)
- Cumulative Page Views 65265  | Unique Visitors 37316
- Dual Language > 
	- [Advanced Features: Internationalized Routing | Next.js](https://nextjs.org/docs/advanced-features/i18n-routing)
		- [Translate website content using Next.js internationalization and next-i18next - YouTube](https://www.youtube.com/watch?v=H9O9HdKNytc)
	- [React.i18next](https://react.i18next.com/)
		- [Go international with your next app: Using i18next to add multilingual support to your React App - YouTube](https://www.youtube.com/watch?v=baLjPx_wFi4)
	- [Imperative API | Format.JS](https://formatjs.io/docs/react-intl/api)
		- [Add Multiple Languages in React Apps | Internalization Basics - YouTube](https://www.youtube.com/watch?v=J0dij6eufOY)
#### 2. Experience
#### 3. Accomplishments (Certification)
#### 4. Blogs
- Temp Posts: Other platforms
- Read More (Link to **Blog Site** > Archive [Halfrost's Field | 冰霜之地](https://halfrost.com/))
- Blog Page
	- Time Read
	- Date Created
	- Tags
	- Author
	- Share this post
	- Related Blogs
	- Comment
#### 5. Books (Publication)/ Documentation
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
#### 6. Projects
- Link to **Github repo**/ demo page ([Github/halfrost](https://github.com/halfrost))
#### 7. Talks (Channel)
- Link to channel page 
- Link to slide page ([halfrost (@halfrost) on Speaker Deck](https://speakerdeck.com/halfrost/))
#### 8. Skills
#### 9. Contact
- [[Blogs and Social Platforms]]

### Tech Architecture Diagram

### Table-Schema Design

## Development (Quality and Efficiency)
- How to build a React Portfolio Website in 15 days?
#### 1. Building Reusable UI Components 
- [x] Archive/ Timeline
- [x] Dynamic visitor data and feedback
	- Cumulative Page Views 65265  | Unique Visitors 37316
- How to use React Component, Hooks?
- [[UI Componenet Library]]
- [[React]] 组件化和 hooks 封装 (复用)
#### 2. [[Testing]]
- Jest
- Storybook
- Joint Debugging 联调 (多人协作效率)
- Unit Test 单元测试 （代码帮你测试代码）
- Monitor 监控报警 （线上问题提前预支）
#### 3. [[Deploying]]
#### 4. Back-End
- [[Database]] 
- [[Server-Side Frameworks]]
- [[Authentication]]
- [[User Analytics]]
#### 5. [[Performance Optimization]]
## Prep Basics - Next.js, TailwindCSS, Sanity
#### 1. Front-End Framework, Tools
- Why do I choose the tech-stack/tools?
- 前端：[[React]], [[Next.js]], [[TypeScript]], 
- 样式：[[Tailwind CSS]]
- 后端：[[Sanity]] > `Groq`
- 基础：[[HTML]], [[CSS]], [[JavaScript]]
- 开发工具：
	- prettier
	- eslint
	- react-code-snippets
- 代码 Review ( 多人协作规范)
- 规范 (统一代码、Git 风格、开发规则) ...
#### 2. Git Repository Set Up
- Pull <u>the new one</u> from remote
- Push <u>the local v1</u> to the remote
- [[Git commands]]
#### 3. Project Initiation 
- 脚手架 （多个项目初始化效率）
##### 3.1. Install NextJS, TailwindCSS
- [[How to start a React, NextJS and TailwindCSS project]] (Configuration and Toolchain)
##### 3.2. Install Sanity CMS 
- [[Sanity]]
##### 3.3. Install Dependencies with Node and NPM
- [[Dependency Installation Error]]
#### 4. GitHub Version Control and Contribute
- How to contribute to a git repo?
## Milestones
- [[2023-02-21]] Build up the initial [[Next.js]] front-end and [[Sanity]] backend for [[Portfolio-个人主页]]
- [[2023-02-16]] Start building my [[Portfolio-个人主页]] website with [[React]] and initiate a git repository for the project
## Logs

```dataview
TABLE title, started, status
WHERE contains(title, "Portfolio")
SORT file.cday DESC
```