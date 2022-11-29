---
title: TechBlog 双语博客立项说明
tags: 项目/TechBlog
status: Done
started: 2022-11-01
closed: 2022-11-11
aliases: 
---
## 项目计划
思考以下问题：
- TechBlog 产品设计、项目目的
- 现有哪些方案，利弊、可行性？
- 开发流程设计
## 项目介绍
A bilingual Tech Blog website with quality translation support.
支持高质量翻译的技术博客网站
#### 目标用户 Target Users
- 想阅读英文技术博客并提升英语的非英语母语开发者
- Non-native English Speaking Developers who would like to read English tech blog and improve English
#### 核心功能 Core Functions
- Users can search and find **Front-end Tech Blog** in the language they preferred
- Users can read the tech blog in its **source language** and choose to read translated version in their **preferred language**
#### ❌ 提供什么内容/价值？
#### ❌ 内容从何而来？
#### ✅Demo
## 同类项目分析
#### 中文技术博客社区：
- 掘金：[https://juejin.cn/](https://juejin.cn/)
- CSDN：[https://www.csdn.net/](https://www.csdn.net/)
#### 英文技术博客社区：
- Medium：[https://medium.com/](https://medium.com/)
- Hashnode：[Explore trending blogs](https://hashnode.com/explore/blogs?category=week)
- Dev.to：[https://dev.to/](https://dev.to/)
#### 个人博客网站
[https://www.vipyubai.top/](https://www.vipyubai.top/)
[https://www.vipyubai.top/](https://www.vipyubai.top/)
[https://yuridevat.hashnode.dev/](https://yuridevat.hashnode.dev/)
## 项目设计灵感
![](https://cdn.nlark.com/yuque/0/2022/png/29677165/1667311541614-0c6ce878-5156-4f43-bae1-6610775f30b6.png)
![](https://cdn.nlark.com/yuque/0/2022/png/29677165/1667960934996-a852b398-ea48-467e-bdfb-03b2f36bcf59.png)
## 核心功能分析与前端技术实现
### 主页
- 主图效果：轮播图
- 注册、登录
- 预览方式：
  - 关键词搜索
  - 博文推荐：最新、最热（阅读排行榜）、置顶
  - 标签搜索：”内容标签“、”定制标签“
  - 分页浏览/ 加载更多
- 博文卡片：
  - 样式：标题、图片、内容描述（图片懒加载）
  - 信息：阅读时长、作者、发布时间、主题标签
  - 数据：浏览量、点赞数、评论数、收藏数……
- 其他信息
  - 二维码：APP，公众号，视频号
  - 友情链接
  - 访问人数
### 导航组件
- 顶部/ 侧边导航栏：固定、平滑滚动定位（待优化）
### 阅读页
- 富文本内容展示（待优化）
- 大纲阅读
- 相关文章、下一篇
- 评论功能：
  - 评论更新、评论数目（待优化）
  - 视频/图片大文件上传及展示
- 收藏
- 点赞
- 分享
- 作者简介、关注
### 写作页
- 写作、编辑、发布功能
### 文章/用户数据可视化：
- 时间线、折线图、饼状图、日历
### 亮点功能
- ⭐ 语言切换
- ⭐ 双语阅读
- ⭐ 自动翻译
- ⭐ 翻译校正
## 项目开发思路
- 模仿 > 设计优化 > 创新
- 侧重：前端 GUI 页面的实现（夯实前端技术基础和核心能力）
## 技术方案调研：React.js, Next.js, Tailwind CSS, Sanity CMS...
### 开源项目/教程：
- Medium-Clone：[YouTube- Medium-Clone-2.0](https://www.youtube.com/results?search_query=build+medium+clone) (内容预览、展示、评论；页面布局)
- Twitter-Clone: （注册、登录、图片上传及展示、评论优化；页面布局）
- TikTok-Clone:（点赞、收藏、视频上传及展示、标签搜索；页面布局）
- NetFlix-Clone: （支付；页面布局）
### 技术难点
- **JS**
  - 数据结构 (Array, Object)、OOP、JSON
  - **后台数据获取及推送**、页面路由、页面渲染、HTML template
- CSS:
  - 布局、样式（字体、颜色）、图片、形状、动画；
  - 代码结构规范：框架
  - 优先级原理
- HTML：
  - SEO
  - 语义化标签
- TS：数据类型
- React: 原理、功能、组件/库
- Next.js: 原理、功能、组件/库， [https://nextjs.org/blog/next-13](https://nextjs.org/blog/next-13) (Oct 26, 2022)
- MVC/ MVVM
## 其他方案调研
### 方案一：CSS, HTML，原生 JS, jQuery...
#### 开源项目/教程：
- [YouTube- JS, jQuery- Blog](https://www.youtube.com/watch?v=gZHjMVE_e10&t=1531s)
#### 技术难点：
### 方案二：CSS, HTML，原生 JS, + Node.js, MongoDB, Mongoose..
#### 开源项目/教程：
- [YouTube-Node.js, MongoDB- Blog](https://www.youtube.com/watch?v=1NrHkjlWVhM&list=RDCMUCFbNIlppjAuEX4znoulh0Cw&start_radio=1&t=138s)
#### 技术难点：
### 方案三：CSS, HTML，原生 JS, + Node.js, Firebase...
#### 开源项目/教程：
- [https://github.com/kunaal438/blogging-site](https://github.com/kunaal438/blogging-site)
#### 技术难点：
**Firebase**
- a container for project
- 11.03 源码页面打开后，上传图片出错 （待解决）
- ![](https://cdn.nlark.com/yuque/0/2022/png/29677165/1667485091901-9b2edcc3-fa69-4434-bcdd-49b89bf1d719.png)
- ![](https://cdn.nlark.com/yuque/0/2022/png/29677165/1667485197971-ff71d1f2-391b-4725-951f-6489f4002ccf.png)
  **Google Analytics**
- a free and unlimited analytics solution that enables targeting, reporting and more in Firebase Crashlytics, Cloud Messaging, in-app messaging, Remote Config, A/B Testing and Cloud Functions.
### 方案五：Vue3 框架 -...
#### 开源项目/教程：
#### 技术难点：
### 模板/低代码建站方案
#### ➖Webflow
#### ➖WordPress
#### ➖Wix
#### ➖hashnode
#### ➖HEXO
- 项目案例：[https://blog.juanertu.com/categories/%E5%8D%9A%E5%AE%A2%E6%90%AD%E5%BB%BA/page/3/](https://blog.juanertu.com/categories/%E5%8D%9A%E5%AE%A2%E6%90%AD%E5%BB%BA/page/3/)
- 教程：[https://www.bilibili.com/video/BV1oU4y1n7hn/?spm_id_from=pageDriver&vd_source=be278a4cfd00a5f72dcf153eaca79333](https://www.bilibili.com/video/BV1oU4y1n7hn/?spm_id_from=pageDriver&vd_source=be278a4cfd00a5f72dcf153eaca79333)
#### 💡PROs & CONs
- 可基于框架、模板快速建站
- 无法通过项目夯实技术基础：HTML, CSS, JavaScript
## 如何部署上线
- CDN 加速
- 服务器
## 项目开发流程
### 技术选型
- 前端
- 后端
- 工具：
  - Webpack/ Parcel
- 测试
- 部署
### 页面搭建
- 主页
  - 确定样式主题：颜色、字体
  - 确定主页内容、布局、组件、样式
  - 运用 HTML, CSS, SASS, JS 基础技术搭建主页雏形，实现基础交互
- 阅读页
  - 确定阅读页内容、布局、组件、样式
  - 运用 HTML, CSS, SASS, JS 基础技术搭建主页雏形，实现基础交互
- 创作页
  - 确定创作页内容、布局、组件、样式
  - 运用 HTML, CSS, SASS, JS 基础技术搭建主页雏形，实现基础交互
- 用户页
  - 确定用户页内容、布局、组件、样式
  - 运用 HTML, CSS, SASS, JS 基础技术搭建主页雏形，实现基础交互
- 注册、登录窗口
### 数据库
- 用户数据
- 博客数据
- 图片管理
### 确定 API 接口
- 双语博客数据：如何获取博客内容？
- 翻译接口：如何设置自动翻译？
- Markdown 识别与编辑器
- 注册接口
- 评论接口
