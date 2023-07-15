---
Title: 怎样实现进度条自动追踪-MetaEdit
tags: PKM
DateModified: 2023-05-09
DateDue:
DateStarted: 2023-04-27
status: ⤵️Snooze
Completed: 2
Incomplete: 0
Total: 2
Progress: 100%
---

- [x] 怎样实现进度条自动追踪 ✅ 2023-05-09
- [x] Test ✅ 2023-05-09

`="<progress  value=" + this.Completed +" max="+ this.Total+"></progress> "+this.Completed+"/"+ this.Total`  
`$= const value = ((dv.current().file.tasks.where(t => t.completed).length) / (dv.current().file.tasks).length || 0) * 100; "<progress value='" + value.toFixed(1) + "' max='100'></progress>" `
