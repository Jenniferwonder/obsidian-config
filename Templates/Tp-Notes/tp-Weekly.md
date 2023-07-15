# {{date:[Week] ww}} [[{{date:YYYY-MM}}|🪴]] {{date:MMM gggg}}
M [[{{monday:gggg-MM-DD}}|{{monday:DD}}]] · T [[{{tuesday:gggg-MM-DD}}|{{tuesday:DD}}]] · W [[{{wednesday:gggg-MM-DD}}|{{wednesday:DD}}]] · T [[{{thursday:gggg-MM-DD}}|{{thursday:DD}}]] · F [[{{friday:gggg-MM-DD}}|{{friday:DD}}]] · S [[{{saturday:gggg-MM-DD}}|{{saturday:DD}}]] S [[{{sunday:gggg-MM-DD}}|{{sunday:DD}}]] ^w{{date:ww}}
## Intentions
```tasks
(happens in <% tp.date.now("YYYY-[W]WW") %>)
group by tags
sort by status
```
## Overview
### Workout
```dataview
TABLE WITHOUT ID
	file.link AS "Day",
	GymTime As "⏰",
	Breast, Back, Abs, Hips, Arms, Legs, Aero
FROM "OKRTs/Daily"
WHERE Week = [[<% tp.date.now("YYYY-[W]WW") %>]]
SORT file.name ASC
```
### Habits
```dataview
TABLE WITHOUT ID
	file.link AS "Day",
	Anki AS "📇",
	Revision AS "🔁",
	Coding AS "⌨️",
	Love AS "❤️",
	MorningExercise As "🧘‍♀️",
	Strength AS "🏋️",
	Aerobics AS "🏃‍♀️",
	Dance As "💃",
	EveningExercise As "🌖"
FROM "OKRTs/Daily"
WHERE Week = [[<% tp.date.now("YYYY-[W]WW") %>]]
SORT file.name ASC
```
### Statistics
```dataviewjs
const daysPath = dv.current().file.folder;
const attributes = {
	'Food': {
		label: 'Food',
		backgroundColor: 'rgba(85, 174, 229, 0.2)',
		borderColor: 'rgba(85, 174, 229, 1)',
		average: 100,
	},
	'Transport': {
		label: 'Transport',
		backgroundColor: 'rgba(101, 213, 218, 0.2)',
		borderColor: 'rgba(101, 213, 218, 1)',
		average: 100,
	},
	'Growth': {
		label: 'Growth',
		backgroundColor: 'rgba(189, 230, 191, 0.2)',
		borderColor: 'rgba(189, 230, 191, 1)',
		average: 1000,
	},
	'LunchAtHome': {
		label: 'LunchAtHome',
		backgroundColor: 'rgba(255, 211, 101, 0.2)',
		borderColor: 'rgba(255, 211, 101, 1)',
		average: 10,
	},
	'Weight': {
		label: 'Weight',
		average: 100,
	},
};

const date = "<% tp.date.now('YYYY-MM-DD') %>";

customJS.DvCharts.renderWeeklyChart({
	dv,
	context: this,
	daysPath: 'OKRTs/Daily',
	attributes,
	type: 'average',
	date
})
```

```dataview
TABLE WITHOUT ID
	link(file.name) as "Day",
	Food AS "🍙",
	Transport AS "🚈",
	Growth AS "📈",
	Weight As "💪",
	LunchAtHome AS "🍚"
FROM "OKRTs/Daily"
WHERE Week = [[<% tp.date.now("YYYY-[W]WW") %>]]
SORT file.name ASC
```
## Actions
- [[<% tp.date.weekday("YYYY-MM-DD", 0) %>|Monday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 0) %>#^actions]]
- [[<% tp.date.weekday("YYYY-MM-DD", 1) %>|Tuesday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 1) %>#^actions]]
- [[<% tp.date.weekday("YYYY-MM-DD", 2) %>|Wednesday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 2) %>#^actions]]
- [[<% tp.date.weekday("YYYY-MM-DD", 3) %>|Thursday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 3) %>#^actions]]
- [[<% tp.date.weekday("YYYY-MM-DD", 4) %>|Friday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 4) %>#^actions]]
- [[<% tp.date.weekday("YYYY-MM-DD", 5) %>|Saturday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 5) %>#^actions]]
- [[<% tp.date.weekday("YYYY-MM-DD", 6) %>|Sunday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 6) %>#^actions]]
## Summary
**[[{{date:YYYY}}-W{{date:ww}}|WEEK {{date:ww}}]]** | **{{sunday:MMM D}}–{{saturday:MMM D}}**
