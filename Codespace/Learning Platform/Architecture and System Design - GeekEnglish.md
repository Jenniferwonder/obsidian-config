---
title: Architecture and System Design - GeekEnglish
tags: Coding-Projects/GeekEnglish 
due: 
started: 2023-03-14 Tue
modified: 2023-03-20 Mon
status: 
---
## Tech Choices 
#### 1. Why & Why not > Demo
#### 2. Front-End Frameworks
- [[React]]
- [[SSG Frameworks]]
##### 2.1. UI Component
- UI Framework/ Libraries
	- [[Tailwind CSS]]
	- [[UI Componenet Library]]
##### 2.2. [[Data Request]]
- [[Next.js]] > `next/router` / `next/link`
	- Connect with [[Sanity]]
	- Connect with [[MongoDB]]
	- Connect to a Backend using [[MongoDB]]?
	- Connect to a Backend using MySQL?
- React Router?
#### 3. Back-End Frameworks
##### 3.1. Database/ Data Store
- [[MongoDB]]
	- Why? > [Comparing The Differences - MongoDB Vs MySQL | MongoDB](https://www.mongodb.com/compare/mongodb-mysql) 
	- Username: Jenniferwonder
	- MM: mCyj7qiT9ntjxl0h
- [[Mongoose]]
- Data Format
	- Picture/ Music/ Video
	- Markdown > HTML
	- User
	- Author
	- Post
	- Quiz
	- Tags
##### 3.2. Back-End Logic > Create API
- [[Node.js and Package manager]]
- Express.js
- [[API Resources]] > [[GraphQL]]
##### 3.3. [[Authentication]]
##### 3.4. [[User Analytics]]
#### 4. [[Testing]]
- Jest
- React Testing Library
#### 5. [[Performance Optimization]]
- Performance monitoring 
#### 6. [[Deploying]]
- [[CI-CD]]
- Server > Vercel/ Netlify/ Github
- [[DNS]]
- CDN
- 备案
#### 7. Dependency
- [[Dependency Installation Error]]
##### 7.1. Dev Tools
- Code Format：
	- prettier
	- eslint
- Efficiency
	- react-code-snippets
	- auto-import
- 代码 Review ( 多人协作规范)
	- Commit standard
#### 8. GitHub Version Control
- Set up a Git repo 
- How to contribute to a git repo?
## Resources Prep
#### 1. [[DNS]]
#### 2. [[Server]]
- Storage
- Bandwidth
#### 3. [[Database]]
#### 4. Object Storage
#### 5. [[CDN]]
#### 6. [[API Resources]]
- Github
- Wechat
- SMS
#### 7. Assets& File Storage
#### 8. Infrastructure as Code (IaC)
- Terraform
- CloudFormation
- Pulumi
## System Design 
只用语言、图描述系统，不写代码  
### 功能模块图 
- [[UML]] / Flow Charts/ Mindmap
- 分为哪些功能模块，功能模块图 (类似流程图或者思维导图)
- 从整体到局部，从大到小，比如（用户前台，管理后台）-》（XX，XX。。）、（XX，XX。。）
- 功能间关系不大的可用思维导图
### 技术架构图
- 更加清晰地展示项目用到了哪些技术，便于后期扩展和改造，起到对项目宏观地指导意义
### 库表设计 (关键)
#### 1. Markdown in DB Solutions?
- [How do you save markdown in database and render it? | Makerlog](https://getmakerlog.com/discussions/waptik-how-do-you-save-markdown-in-database-and-re)
##### 1.1. MD Editor/Render/Parser (Convert .md to HTML)
- [GitHub - HarryChen0506/react-markdown-editor-lite: a light-weight Markdown editor based on React. 一款轻量的基于React的markdown编辑器](https://github.com/HarryChen0506/react-markdown-editor-lite)
- [GitHub - markdown-it/markdown-it: Markdown parser, done right. 100% CommonMark support, extensions, syntax plugins & high speed](https://github.com/markdown-it/markdown-it)
##### 1.2. Raw markdown files in folders not in DB?
- User created .md input?
- Other items of a blog post? (title, date, description, cover, tag, author)

1. 对着 **需求信息表** ([[Requirement Table]])
2. 划分哪些库 - 每个项目一个库
3. 划分哪些表 - 每个大的功能一个表
4. 确定每个表有哪些字段
5. 养成存储建表语句的习惯
6. 表之间的关联关系（通过字段约定式关联）
7. 反三范式
8. 设计很重要，前期要确定字段，后期避免上线库加字段 (可能会锁表，查询卡死)
9. 必要的四件套字段
10. id(int)、create_time(current_timestamp)、update_time(current_timestamp 并且加 on update current_timestamp)、isDelete（软删除，逻辑删除）
11. 将设计清晰地记录下来
### 每个功能的实现逻辑
1. 每个需求详细设计
2. 结构怎么设计
3. 流程越详细越好
- Specific Function/ Component Develepment Plan
	- Requirement and background
	- Implementation Steps/ Logic
## Development Standards
#### 1. Coding Convention/ Style Guide 
编码规范很重要，架构师维持编码规范的几种方式
1. 人为约定 (Alibaba Java 开发手册等等)
2. 工具：插件 
	- 后端 idea 的 alibaba java coding guide 、checkstyle、
	- 前端的 Eslint 等
#### 2. Submission Standard
1. 提交规范 (隐私保护)
2. 同一的提交记录，比如关联需求文档
3. 忽略某些文件的提交，保护隐私，可用使用.gitignore
## Requirement Fulfilling Schedule
1. 先做需求评估和设计
2. 排期稳一点，比预期时间多一些
3. 预留时间改 bug
4. 排期前预估和提出风险  

