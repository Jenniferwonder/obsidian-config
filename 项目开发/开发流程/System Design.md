---
title: System Design
tags: Projects/Workflow
status: Done
modified: 2023-03-07 Tue
started: 2022-10-31 
due: 
aliases: 
---
## Architecture Overview
[The Benefits of Functional Architectures | Systems Engineering, Part 3 - YouTube](https://www.youtube.com/watch?v=UTm1ORuZ1dg)
![[Pasted image 20230308083747.png]]
#### 1. Functional Architecture
![[Pasted image 20230308091015.png]]
##### 1.1. Function Decomposition
- Verb-Noun Pairing
	- ![[Pasted image 20230308091126.png]]
- Back and forth between engineering team and stakeholders (Needs under speficified)
- 
### Basics
[Getting the Basics - Software Architecture Introduction (part 1) - YouTube](https://www.youtube.com/watch?v=8UlLgOf20Ho)  
Functional Requirements
- Maintainability
- Scalability
- Reliability
- Efficiency
Restrictions
Priorities
- Time to market vs Features
- Portability vs Scalability/ Maintainability
Layered Architecture
- UI
	- Presentation Layer
- Logic
	- Business Layer
	- Persistence Layer
- Store
	- Database Layer
## Web App Architecture
[WEB APP ARCHITECTURE - THE ULTIMATE APPROACH!! - YouTube](https://www.youtube.com/watch?v=PjprIvgGh90)
![[Pasted image 20230307214310.png]]
### Server-side development approaches
#### 1. Monolithic Architecture 单体应用
[Monolithic架构到微服务 - 腾讯云开发者社区-腾讯云](https://cloud.tencent.com/developer/article/1349624)
[Monolithic vs Microservices Architecture - Which One Is Right for You?Jelvix](https://jelvix.com/blog/monolith-vs-microservices-architecture)
![[Pasted image 20230307215154.png]]
Single codebase but risky for highly scalable platforms
#### 2. Microservices
- Isolation
- Scalability
- Flexibility
- Simplified development
##### 2.1. Disadvantage
- need for secure algorithm
- challenge of breaking the architecture into smaller features
#### 3. Serverless 
Use servers to run a web app, which are not hosted by the company
- Don't care about the server
- pay for used server space only
- tech support
#### 4. Best Practices
1. Find a solution that covers most of your goals
2. Choose the simplest option with minimalistic architecture
3. Keep your architecture lightweight
4. Your architecture should be able to identify and repair issues on its own
5. Automate process
6. Pay attention to Data Storing
### Client-side development approaches
#### 1. [[Service Worker-PWA]]
#### 2. SPA
#### 3. MPA
- Complex backend development
- Lower performance speed
- Complicated debugging
## System Design
[System Design for Beginners Course - YouTube](https://www.youtube.com/watch?v=m8Icp_Cid5o)
### Design Patterns
A general **reusable solution** to a commonly occuring problem within a given context in software design.
Convert business requirements into technical solutions
#### 1. Publisher-subscriber model
[Systems Design Interview Concepts (for software engineers / full-stack web) - YouTube](https://www.youtube.com/watch?v=REB_eGHK_P4)  
- Load Balancing
- Caching
- CDN
- Replication
- [[Database]] 
- API Design
创作时间：2022 年 10 月 31 日
## **第二天：如何做好架构师**
00:00:00~00:06:53 组队安排 (看回放的同学直接跳过)  
00:06:54~00:25:20 项目点评 (看回放的同学直接跳过)
### 00:25:21~00:26:50 提出问题：如何做好架构师？
1. 架构师的定义
2. 技术负责人要做好哪些事情
3. 技术选型
4. 资源准备
5. 系统设计
6. 开发规范
7. 需求排期
### 00:26:51~00:30:10 00:34:11~00:56:45 如何做好技术选型？
技术选型两步走
1. 1、选
2. 系统开发
3. 前端、后端、上线的方式
4. 工具链
5. 开发、测试、上线工具
6. 技术选型原则：
7. 看人：团队对哪个技术最熟？有没有一个技术大佬
8. 看需求：
9. 项目的量级？大项目考虑扩展性 (百万并发、消息队列、分库分表)，小项目尽量简单
10. 项目的功能？
11. 尽量用热门技术
12. 技术选型渠道
13. 搜解决方案：掘金、GitHub、openbase（前端）
14. 百度开发者搜索 
15. 星球内鱼皮对系统设计的回答
16. 第三方平台（直播、短信、视频点播、第三方存储、OCR 文字识别等）
17. 数据库选型
18. 思考数据量级
19. 思考数据的应用场景 (数据间联系等)
20. 2、用
21. 能在技术选型阶段确认的技术尽量提前确认，怎么确定技术可以用呢？
22. 看文档确认版本号
23. 先跑起来一个 demo，跑起来没问题再确认技术选型
### 00:56:46~01:15:10 资源准备
资源包括：服务器、数据库、第三方服务（短信发送）、开发软件等  
开发最省钱的方案：
1. 服务器指标
2. 带宽、内存、服务器 CPU、硬盘
3. 带宽计算：计算每秒访问的总资源大小（人数 _ 单位资源大小 (比如打开一次网页的带宽消耗)）_ x 2
4. 内存估算：本地开发时查看进程占用，或者在 linux 部署运行查看 (top 命令)
5. 服务器 CPU：核心数
6. 硬盘大小、云数据库
7. 团队资源文档/表
### 01:15:11~01:48:30 系统设计
只用语言、图描述系统，不写代码  
系统设计：
1. **功能模块图** 
	- [[UML]]
	- Process Flow Charts
2. 分为哪些功能模块，功能模块图 (类似流程图或者思维导图)
3. 从整体到局部，从大到小，比如（用户前台，管理后台）-》（XX，XX。。）、（XX，XX。。）
4. 功能间关系不大的可用思维导图
5. **技术架构图**
6. 更加清晰地展示项目用到了哪些技术，便于后期扩展和改造，起到对项目宏观地指导意义
7. **库表设计** (关键)
8. 对着 **需求信息表**
	- ![[Pasted image 20230307175909.png]]
9. 划分哪些库 - 每个项目一个库
10. 划分哪些表 - 每个大的功能一个表
11. 确定每个表有哪些字段
12. 养成存储建表语句的习惯
13. 表之间的关联关系（通过字段约定式关联）
14. 反三范式
15. 设计很重要，前期要确定字段，后期避免上线库加字段 (可能会锁表，查询卡死)
16. 必要的四件套字段
17. id(int)、create_time(current_timestamp)、update_time(current_timestamp 并且加 on update current_timestamp)、isDelete（软删除，逻辑删除）
18. 将设计清晰地记录下来
19. 每个功能的实现逻辑
20. 每个需求详细设计
21. 结构怎么设计
22. 流程越详细越好
### 01:48:31~02:08:23 开发规范 (非常非常重要)
1. 编码规范很重要，架构师维持编码规范的几种方式
2. 人为约定 (Alibaba Java 开发手册等等)
3. 工具：插件 后端 idea 的 alibaba java coding guide 、checkstyle、前端的 Eslint 等
4. 提交规范 (隐私保护)
5. 同一的提交记录，比如关联需求文档
6. 忽略某些文件的提交，保护隐私，可用使用.gitignore
### 02:08:24~02:12:15 需求排期
1. 先做需求评估和设计
2. 排期稳一点，比预期时间多一些
3. 预留时间改 bug
4. 排期前预估和提出风险  
02:12:15~02:16:59 组队安排 + 回答问题 (看回放的同学跳过)
