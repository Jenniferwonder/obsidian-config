---
title: Daily Plan
tags: 学习记录/周
started: 2023-01
due: 2023-01
modified: 
status: Doing
---
# Daily Plan
## 今日目标
#### 1. [[Questions#🚀TECH| Tech]]
- **[[React]]** 技术总结、应用与提升
#### 2. [[Questions#🚀PROJECT|Project]]
- [[React 项目案例]] 总结
#### 3. [[Questions#🌍ENGLISH|English]]

## 今日收获
### ✍️创建笔记
```dataview
TABLE title, started, status
WHERE file.cday = date(2023-01-09)
SORT file.mday DESC
```

### 📝完善笔记

```dataview
TABLE title, started, status
WHERE file.mday = date(2023-01-09) AND file.cday != date(2023-01-09) AND contains(modified, "2023-01-09")
SORT file.mday ASC
```
### 🌍English-Time
```dataview
TABLE title, started, status
WHERE tags = "英语学习"
SORT started ASC
```
### 🗺️Graph View of Today

## 反思提升
- [ ] 
## 任务追踪
### Morning Prep
- [ ] 07:30 Note Review/Update
- [ ] 08:40 Breakfast
### Morning Task
- [ ] 09:20 Note Review/Update
- [ ] 12:20 Lunch
### Afternoon Task
- [ ] 13:00 Tech & Project
- [ ] 16:30 English-Time
- [ ] 18:30 Dinner
### Evening Break
- [ ] 19:00 Reflection
	- [ ] Graph View of Today
	- [ ] 反思提升
	- [ ] Update Template 
- [ ] 20:00 笔记备份 `ALT + G`
- [ ] 20:30 BREAK