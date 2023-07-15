---
Title: Daily Plan
tags: Daily
DateStarted: <% tp.date.now("YYYY-MM-DD") %>
DateModified: <% tp.date.now("YYYY-MM-DD") %>
---
# Daily Plan
- Week:: [[<% tp.date.now("YYYY-[W]WW") %>]]
- Next:: 
- WakeUp:: 
- Linked:: [[DV-Tasks]]
## Tasks
### Todo
```tasks
not done
(happens on  <% tp.date.now("YYYY-MM-DD") %> ) OR (due before in 5 days)
sort by due
```
### Done
```tasks
done
(done on  <% tp.date.now("YYYY-MM-DD") %>)
```
## Actions
## Trackers 
### Statistics 
- Weight::
- Food:: 
- Transport:: 
- Growth::
- LunchAtHome:: 
### Habits
- Love::
#### 1. Workout
- GymTime::  
- Stretch::
- Aerobics:: 
	- Aero:: 臀圆机
- Strength:: 
	- Breast:: 扩胸机
	- Back:: 引体向上, 划船机
	- Abs:: 卷腹机, 腹旋转机
	- Hips:: 臀外展机
	- Arms:: 引体向上, 哑铃
	- Legs:: 上抬腿
- Dance::
#### 2. Study
- StudyTime::
- Anki::
- Revision::
- Coding:: 
- Reading::
### Outcomes
- TechSkills::
- PKM:: 
- PMP:: 
- CPE::
- Life:: 
## Review
- ToImprove::  
### ✍️New Notes

```dataview
TABLE title, DateStarted, status
WHERE DateStarted = date(<% tp.date.now("YYYY-MM-DD") %>)     
SORT file.mday DESC
```

### 📝Modified Notes

```dataview
TABLE title, DateStarted, status
WHERE file.cday != date(<% tp.date.now("YYYY-MM-DD") %>) AND DateModified = date(<% tp.date.now("YYYY-MM-DD") %>)
SORT modified ASC
```
