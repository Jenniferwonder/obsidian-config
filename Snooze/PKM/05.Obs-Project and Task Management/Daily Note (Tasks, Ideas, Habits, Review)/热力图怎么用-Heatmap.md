---
Title: 热力图怎么用-Heatmap
tags: PKM
DateStarted: 2023-04-27
DateModified: 2023-05-27
status: ⚪Backlog
aliases: Heatmap Calendar
Progress: NaN%
---

Heatmap Calendar  
热力图怎么用

- 追踪目标、习惯、任务、运动、财务等
```dataviewjs
dv.span("**🏋️ Exercise 🏋️**")
const calendarData = {
    year: 2023,
    colors: {
        red: ["#ff9e82","#ff7b55","#ff4d1a","#e73400","#bd2a00",]
    },
    entries: []
}

for(let page of dv.pages('"000-OKRTs/Daily"').where(p=>p.read)){
    calendarData.entries.push({
        date: page.file.name,
        intensity: page.read,
        content: await dv.span(`[](${page.file.name})`), //for hover preview
    })
       
}

renderHeatmapCalendar(this.container, calendarData)

```

```dataviewjs
dv.span("**💸 Pages Read 💸** (11 intensities instead of 5)")
const calendarData = {
		year: 2023,
		colors: "green",
    entries: [],
}
for(let page of dv.pages('"000-OKRTs/Daily"').where(p=>p.pageRead)){
    calendarData.entries.push({
        date: page.file.name,
        intensity: page.pageRead,
        content: await dv.span(`[](${page.file.name})`), //for hover preview
    })  
}
renderHeatmapCalendar(this.container, calendarData)
```