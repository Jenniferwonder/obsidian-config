---
title: Date
tags: Coding/JS
started: 2022-12-01 Thu
due: 
modified: 2022-12-01 Thu
status: 
number headings: auto, first-level 4, max 6, 1._.1.1.
---
#### 1. Get Current date and time
```JS
new Date( )
new Date(2022, 10, 19, 15, 23, 5)
//JS month starts from 0
//return '2022 Nov 19 15:23:05'
```
#### 2. Time stamp
##### 2.1. get the current time stamp
```JS
Date.now()
currentTime = new Date()
currentTimeStamp = currentTime.getTime()
```
##### 2.2. convert a time stamp to a time
```JS
.getTime(`timeStamp/ mileseconds`)
```
##### 2.3. convert a timestamp to a date
```JS
new Date(`timestamp`)
```
#### 3. Get the number of day passed from the current date
```js
Math.round(Math.abs(date - new Date( ))/ (1000 * 60 * 60 * 24))
```
#### 4. Get elements of Date
```JS
.getFullYear
.getMonth
.getDate
.getDay
.getHours
.getMinutes
.getSeconds
```
#### 5. Change elements of Date
```js
.setFullYear(2040)
.set...
```
#### 6. Internationalizing Dates
```js
new Intl.DateTimeFormat('en-US').format(new Date())
// Options
new Intl.DateTimeFormat('en-US', Options).format(new Date())
Options = {hour: 'numeric', minute: '', day:'', month: 'long/ 2-digit', year:'', weekday: 'long/ short/ narrow',}
```
##### 6.1. ISO Language Code Table:
www.lingoes.net
##### 6.2. Get the browser language
```js
navigator.language
```
#### 7. Get a nice formatted Time string
```js
.toISOString
```