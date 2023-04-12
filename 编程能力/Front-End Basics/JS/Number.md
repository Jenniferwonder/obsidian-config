---
title: Number
tags: Coding/JS  
started: 2022-12-01 Thu
due: 
modified: 2022-12-01 Thu
status: 
number headings: auto, first-level 4, max 6, 1._.1.1.
---
## Number Methods
### Convert
- [[Data Types and Data Structures#Type Conversion and Coersion]]
### Parse
#### 1. Parse number from string
```js
Number.parseInt('30px')
//return '30'
Number.parseInt('e23')
//not working
Number.parseInt('30px', 10)
//return '30'
Number.parseFloat('2.5rem')
//return '2.5'
```
### Check
#### 1. Check if value is NaN 🟨
```js
.isNaN('20')
//return "true"
Number.isNaN('20')
//return "false"
Number.isNaN(20)
//return "false"
```
#### 2. Check if value is Number
```js
Number.isFinite( )
```
#### 3. Check if a value is Interger
```js
Number.isInteger( )
```
