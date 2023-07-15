---
Title: Homepage
tags: PKM
DateStarted: 2023-05-04
DateModified: 2023-05-24
---
## OKRTs

````ad-flex
```ad-blank
- ### Areas
- [[Front-End]]
- [[PM]]
- [[PKM]]
- [[CPE]]
- [[Life]]
- [[People]]
```
```ad-blank
- ### Tasks
- ⚡[[DV-Tasks]]
- ⚡[[DV-Due]]
- ⚡[[KB-Tasks]]  
- Gantt Chart
```
```ad-blank
- ### Periodic Notes
- 📆 [[DB-Daily 2023]]
- 📆 [[DB-Daily 2022]]  
- 👁️ [[Daily]]
- [[Habit Tracker]]
```
````

## 2023
```ad-kanban
- **Q1**
	- [[2023-01]]
	- [[2023-02]]
	- [[2023-03]]
- **Q2**
	- [[2023-04]]
	- [[2023-05]]
	- [[2023-06]]
- **Q3**
	- [[2023-07]]
	- [[2023-08]]
	- [[2023-09]]
- **Q4**
	- [[2023-10]]
	- [[2023-11]]
	- [[2023-12]]
```
## Command Center 
````ad-flex
```ad-blank
- `button-suibi2`
```
```ad-blank
- `button-gwrite`
```
````
## Database
```ad-kanban
- **Daily**
	- [[DB-Daily 2022]]
	- [[DB-Daily 2023]]
- **Tasks**
	- [[DB-Projects]]
- **CPE**
	- [[DB-CPE]]
	- [[DB-Resonance]]
	- [[DB-Published]]

```


````ad-flex
<div>

### 最近编辑
```dataview
table WITHOUT ID file.link AS "标题",file.mtime as "时间"
from !"模板" and !"kanban" and !#Daily
sort file.mtime desc
limit 15
```
</div>

<div>

### 三天内创建的笔记
```dataview
table file.ctime as 创建时间
from !#Daily
where date(today) - file.ctime <=dur(3 days)
sort file.ctime desc
limit 15
```
</div>
````