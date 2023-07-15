---
Type: Note
Title: Database-数据库原理
tags: TechSkills
DateStarted: 2023-05-17
DateModified: 2023-06-28
DateDue: 
status:
sr-due: 2023-07-02
sr-interval: 4
sr-ease: 276
---
## Metadata
- Topic:: [[System Fundamentals]]
- Up:: [[Back-End Basics]]

## 数据库原理 Intro 
#### 1. What?
操作系统提供**文件系统**来管理文件数据，而文件比较适合保存连续的信息，如一篇文章、一个图片等。
- 但有时需要保存一个名字等较短的信息。如果单个文件只保存名字这样的几个字节的信息的话，就会浪费大量的磁盘空间，而且无法方便地查询（除非使用索引服务）。  
**数据库**则更适合保存这种短的数据，而且可以方便地按字段进行查询。现代流行的数据库管理系统有两大类：
- SQL（基于 B+ 树，强一致性）
- NoSQL（较弱的一致性，较高的存取效率，基于哈希表或其他技术）。  
#### 2. Why?
- 了解**数据库访问性能调优**的要点
- 以及保证并发情况下数据操作原子性的方法。
#### 3. How?
- 阅读各类数据库图书
- 多做数据库操作以及数据库编程，
- 多观察分析数据库在运行时的性能
## MOCs
%% Begin Waypoint %%
- **[[Database-数据库原理]]**
	- [[Database Choices]]
	- [[Firebase]]
	- [[GraphQL]]
	- [[Headless CMS]]
	- [[JSON]]
	- [[Markdown in DB Solutions]]
	- [[Mock Data]]
	- [[MongoDB]]
	- [[Mongoose]]
	- [[NoSQL Databases]]
	- [[ORMS]]
	- [[Sanity]]
	- [[SQLRelational Databases]]

%% End Waypoint %%
## Reference Links