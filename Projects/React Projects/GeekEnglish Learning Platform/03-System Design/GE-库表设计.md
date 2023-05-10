---
Title: GE-库表设计
tags: GeekEnglish/System
DateStarted: 2023-04-24 Mon
due:
DateModified: 2023-04-24 Mon
status:
---

### Database

- [[Database]]
- [[MongoDB]]
- [[Mongoose]]

### Data Format

- Picture/ Music/ Video
- Markdown > HTML
  - [[Markdown in DB Solutions]]
- User
- Author
- Post
- Quiz
- Tags

## GE-库表设计 (关键)

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
