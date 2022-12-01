---
title: Object
tags: JS
started: 2022-12-01 Thu
due: 
modified: 2022-12-01 Thu
status: 
number headings: auto, first-level 4, max 6, 1._.1.1.
---
## Basics
#### 1. Composition
- key/ property
- value
#### 2. How to access value
- dot
- bracket notation: `[' ']`
#### 3. Destructuring
```js
const {key:`varName`} = variable
//store the property value of an object into a variable based on the property key
```
## Methods
#### 1. ES6 enhanced object literals
- Create [[Function]] as **methods** inside an object
#### 2. Object Built-in Methods
```js
this.
//Refer to the object calling the function (except arrow function in which 'this' refers to its parent object)
Object.assign({}, `objectName`)
//create a new object by merging existing objects together
Object.freeze({})
//make property in the object immutable. i.e. unable to add new properties, but the value inside a deeper level is mutable
//work better in strict mode
```

## Special Objects
#### 1. [[Array]]
#### 2. [[Object]]
#### 3. [[Number]]
#### 4. [[Math]]
#### 5. [[Date]]