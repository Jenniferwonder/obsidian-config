---
Title: 尝试甘特图图示时间进度：Obsidian Mermaid（Gantt Chart）
Type: Note
DateStarted: 2023-04-28
DateModified: 2023-07-04
tags: PKM
status: ⤵️Snooze
---

[Gantt diagrams | Mermaid](https://mermaid.js.org/syntax/gantt.html)  
[Fetching Title#0mtv](https://www.youtube.com/watch?v=rXhUeV5Ko7g&t=625s)

```mermaid
gantt
    title A Gantt Diagram
    dateFormat  YYYY-MM-DD
    section Section
    A task           :a1, 2014-01-01, 30d
    Another task     :after a1  , 20d
    section Another
    Task in sec      :2014-01-12  , 12d
    another task      : 24d
```
