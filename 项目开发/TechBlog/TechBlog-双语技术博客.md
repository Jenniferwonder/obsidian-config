---
title: TechBlog-双语技术博客
tags: Projects/TechBlog
status: Doing
started: 2022-11-17 Thu
due: 2022-11-11
modified: 2022-12-14 Wed
---
## 项目时间
启动时间：2022 年 11 月 1 日  
完成时间：
## 项目计划
思考以下问题：
- TechBlog 产品设计、项目目的
- 现有哪些方案，利弊、可行性？
- 开发流程设计
## 项目介绍
A bilingual Tech Blog website with quality translation support.  
支持高质量翻译的技术博客网站
#### 1. 目标用户 Target Users
- 想阅读英文技术博客并提升英语的非英语母语开发者
- Non-native English Speaking Developers who would like to read English tech blog and improve English
#### 2. 核心功能 Core Functions
- Users can search and find **Front-end Tech Blog** in the language they preferred
- Users can read the tech blog in its **source language** and choose to read translated version in their **preferred language**
#### 3. ❌ 提供什么内容/价值？
#### 4. ❌ 内容从何而来？
#### 5. ✅Demo
## 项目技术需求
#### 1. 前端
- [[JavaScript]]
- [[CSS]]
	- [[Tailwind CSS]]
	- [[SASS]]
- [[React]]
- [[Next.js]]
#### 2. 工具
- Create React App
- [[Vite]]
#### 3. 后端
- 🟩[[Node&Express]]
- 🟩[[MongoDB, Mongoose]]
- [[Sanity]]
- [[Firebase]]
## 同类项目分析
#### 1. 中文技术博客社区：
- 掘金：[https://juejin.cn/](https://juejin.cn/)
- CSDN：[https://www.csdn.net/](https://www.csdn.net/)
#### 2. 英文技术博客社区：
- Medium：[https://medium.com/](https://medium.com/)
- Hashnode：[Explore trending blogs](https://hashnode.com/explore/blogs?category=week)
- Dev.to：[https://dev.to/](https://dev.to/)
#### 3. 个人博客网站
[https://www.vipyubai.top/](https://www.vipyubai.top/)  
[https://www.vipyubai.top/](https://www.vipyubai.top/)  
[https://yuridevat.hashnode.dev/](https://yuridevat.hashnode.dev/)
## 项目设计灵感
![](https://cdn.nlark.com/yuque/0/2022/png/29677165/1667311541614-0c6ce878-5156-4f43-bae1-6610775f30b6.png)  
![](https://cdn.nlark.com/yuque/0/2022/png/29677165/1667960934996-a852b398-ea48-467e-bdfb-03b2f36bcf59.png)
## 核心功能分析与前端技术实现
>参考：[[博客网站功能]]
>[React Node.js Full Stack Blog App Tutorial | MERN Stack APP Full Course - YouTube](https://www.youtube.com/watch?v=LelifxOrzvw&list=PLj-4DlPRT48nfYgDK00oTjlDF4O0ZZyG8&index=8)
### 主页
- 主图效果：轮播图
- 注册、登录
- 预览方式：
	- 关键词搜索
	- 分页浏览/ 加载更多
	- 博文推荐：最新、最热（阅读排行榜）、置顶
	- 标签搜索：”内容标签“、”定制标签“
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
## 技术方案调研
参考：
- [[React, NextJS Projects]]
- [[低代码建站方案]]
## 如何部署上线
参考：
- [[Deploy (CI-CD)]]
## 项目开发思路
- 模仿 > 设计优化 > 创新
- 侧重：前端 GUI 页面的实现（夯实前端技术基础和核心能力）
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
## 项目相关文档

```dataview
TABLE title, started, status
WHERE contains(tags, "TechBlog")
SORT started DESC
```