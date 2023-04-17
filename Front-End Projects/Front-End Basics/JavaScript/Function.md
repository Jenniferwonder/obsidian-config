---
title: Function
tags: Coding/JS
started: 2022-12-01 Thu
due:
modified: 2022-12-01 Thu
status:
number headings: auto, first-level 4, max 6, 1._.1.1.
---
## Reference
>[Functions - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions)
## Overview
![[Pasted image 20230310112955.png]]
## Basics
#### 1. Promp and Alert
```js
promp('')
//get user input
alert()
```
#### 2. Default parameters
#### 3. IIFE
immediately invoked function expression
```JS
(function( ) { } )( );
```
#### 4. Closures
to give a function access to all variables of its parent function, even after that parent function has returned
## Create a function
#### 1. Function declaration 函数声明
Able to call the function before declaring it
```js
funtion funName (parameter> argument) { }
```
#### 2. Function expression 函数表达式
An expression produces a value
```js
const funName = funtion (parameter> argument) { }
```
#### 3. Arrow function (ES6)
- An expression produces a value
- does not have its own "this" key word
- "this" in arrow function refers to its parent object/ function
- can not be constructor function in OOP
## Function Methods 🟨
#### 1. Name
```js
funName.name
//to get the name of the function
```
#### 2. Call
```js
funName.call(`newObjectName`, `function parameter`)
//to apply the function with "this" inside an object to a new object
```
#### 3. Apply
#### 4. Bind
```JS
const newFunName = funName.bind(`newObjectName/ argument to event handlers`)
//create a new function to apply the function with "this" inside an object to a new object
const newFunName = funName.bind(`newObjectName`, `pre-set parameter`)
```
