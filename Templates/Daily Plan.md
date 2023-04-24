---
title: Daily Plan
tags: Study-Log/
started: 
due: 2023-04
modified: 
status: Doing
---
# Daily Plan
## Logs

## What's my problem/question today?

## What're my biggest achievements?
### ✅Achievements

### ✍️New Notes

```dataview
TABLE title, started, status
WHERE contains(started, <% tp.date.now("YYYY-MM-DD") %>)
SORT file.mday DESC
```

### 📝Modified Notes

```dataview
TABLE title, started, status
WHERE started != file.cday AND contains(modified, <% tp.date.now("YYYY-MM-DD") %>)
SORT modified ASC
```

## Where can I improve?
- [ ] 
