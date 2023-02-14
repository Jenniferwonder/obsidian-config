---
title: Object
tags: Front-End/JS
started: 2022-12-01 Thu
due: 
modified: 2022-12-05 Mon
status: 
number headings: auto, first-level 4, max 6, 1._.1.1.
---
## Learning Resources
### Reference
- [Working with objects - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects)
- [Introducing JavaScript objects - Learn web development | MDN](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects)

## What is Object in JS?
- A collection of **Key-Value** Pairs, composed of
	- Key/ Property (属性)- [[Object#Properties]]
	- Value
- A Reference Type- [[Data Types and Data Structures#Reference Type]]
- There are many Built-in Objects in JS- [[Object#2. Built-in Objects in JS]]
- Every Object has a property called 'constructor', refering to the [[Object#3. ✅Constructor(构造器) Function|Constructor Function]] that is used to create that object

```js
let x = {} // let x = new Object{};
// Other built-in constructors and literals
new String(); // '', "", ``
new Boolean(); // true, false
new Number(); // 1, 2, 3...
new Function(`arg`,``) // function(`arg`){}
new Error()
```

## Built-in Objects in JS
>[Standard built-in objects - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects)
- [[Array]]
- [[Object]]
- [[Number]]
- [[Math]]
- [[Date]]
- [[Function]]
- [[JSON]]
- [[Fetch API]] - Request, Response
## How to Create Object?
#### 1. ⛔Object literal (对象字面量) syntax: `{ }`
- [[Value and Variables]]

```js
// Object literal syntax
const circle = {
	radius: 1,
	location: {
		x:1,
		y:1
	},
	draw: function() {
		console.log('draw')
	}
} ;
circle.draw();
```

#### 2. ⛔Factory Function 

```js
// Factory Function
function createCircle(radius){
	return {
		radius,
		draw: function(){
			console.log('draw');	
		}
	};
}
const circle = createCircle(1);
```

#### 3. ✅Constructor(构造器) Function

```js
// Constructor Function
function Circle(radius) {
	this.radius = radius;
	this.draw = function(){
		console.log('draw');	
	}
}
const another = new Circle(1);
```

#### 4. Destructuring 🟨

```js
const {key:`varName`} = variable
//store the property value of an object into a variable based on the property key
```

## Properties
#### 1. Add/ Remove Property
- dot notation (点表示法) `obj.propname = ...`
- bracket notation: `obj['propname'] = ...`
	- can be used when property name is **invalid** to be accessed by dot
	- can be used when property name is **dynamically** changing
- Delete property
	- `delete obj.propname/ obj['propname']`  
#### 2. How to access value?
- dot notation
- bracket notation: `[' ']`
#### 3. How to access key/property?

```js
for (let key in circle) {
	console.log(key, circle[key]); // return key and value
}
const keys = Object.keys(obj); // return an array of keys` 
```

#### 4. Private Properties

```js
function Circle(radius) {
	this.radius = radius;
	// Use 'let' to convert properties into variables only available inside this scope
	let defaultLocation = {x:0, y:0};
	let computeLocation = function(factor) { } 
	// Closure enables the parent function variable is accessble to its child without 'this' keyword 
	this.draw = function(){
		computeLoaction(0.1); 
		console.log('draw');
	};
}
const circle = new Circle(10);
circle.draw();
```

#### 5. Getters/ Setters

```js
{
	Object.defineProperty(this, 'defaultlocation', {
		get: function(){
			return defaultLocation;
		},
		set: function(value) {
			if(!value.x || !value.y)
				throw new Error('Invalid Location');
			defaultLocation = value;
		}
	});
}
const circle = new Circle(10);
circle.defaultLocation = 1; // Return error message
```

#### 6. CASE - Stop Watch
Reference: [[Date]]

```js
// Stopwatch Constructor Function
function Stopwatch(){
	let startTime, endTime, running, duration = 0;
	this.start = function {
		if (running)
			throw new Error('Stopwatch has already started.')
		running = true;
		startTime = new Date
	};
	this.stop = function {
		if(!running)
			throw new Error('stopwatch is not started.');
		running = false;
		endTime = new Date();
		const seconds = ((endTime.getTime() - startTime.getTime()) / 1000;
		duration += seconds;
	};
	this.reset = function {
		startTime = null;
		endTime = null;
		running = false;
		duration = 0;
	};
	Object.defineProperty(this, 'duration', {
		get: function(){ return duration; }
	});
}
// Use Stopwatch
const sw = new Stopwatch()
sw.start
```

## Methods
#### 1. ES6 enhanced object literals 🟨
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