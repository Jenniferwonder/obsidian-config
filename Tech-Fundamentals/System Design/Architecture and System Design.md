---
title: Architecture and System Design
tags: Coding-Projects/Workflow
status: Done
started: 2022-11-22 Tue
modified: 2023-03-13 Mon
due:
---
## Reference
- [[Architecture Methodolody]]
- [[Web Architecture]]
- [[System Design Methodology]]
- [[D2-System Architecture]]
## Tech Stack Choices 
#### 1. Choose
- [[Front-End Tech Stack]]
#### 2. Confirm Choices
- Version available from documentation
- Run **demo** to confirm choices
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
#### 1. 功能模块图 
- [[UML]] / Flow Charts/ Mindmap
- 分为哪些功能模块，功能模块图 (类似流程图或者思维导图)
- 从整体到局部，从大到小，比如（用户前台，管理后台）-》（XX，XX。。）、（XX，XX。。）
- 功能间关系不大的可用思维导图
#### 2. 技术架构图
- 更加清晰地展示项目用到了哪些技术，便于后期扩展和改造，起到对项目宏观地指导意义
#### 3. 库表设计 (关键)
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
#### 4. 每个功能的实现逻辑
1. 每个需求详细设计
2. 结构怎么设计
3. 流程越详细越好
- Single Function/ Component Develepment Plan
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

