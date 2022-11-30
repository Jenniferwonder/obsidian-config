---
title: Daily Plan
tags: 学习记录/周
started: 2022-11
due: 2022-11
modified: 
status: Doing
---
# Daily Plan
## 今日目标
#### ❓[[Questions]]
1. 
## 今日收获
### ✍️创建笔记
```dataview
TABLE title, started, status
WHERE file.cday = date(2022-12-01)
SORT file.mday DESC
```

### 📝完善笔记

```dataview
TABLE title, started, status
WHERE file.mday = date(2022-12-01) AND file.cday != date(2022-12-01) AND contains(modified, "2022-12-01")
SORT file.mday ASC
```
### 🌍English-Time
```dataview
TABLE title, started, status
FROM "English-Time"
WHERE started = "2022-11-29 Tue"
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