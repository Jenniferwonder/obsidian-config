---
title: Math
tags: Coding/JS
started: 2022-12-01 Thu
due: 
modified: 2022-12-06 Tue
status: 
number headings: auto, first-level 4, max 6, 1._.1.1.
---
>[Math - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math)  
>[Basic math in JavaScript — numbers and operators - Learn web development | MDN](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Math)
## Math Methods
#### 1. Random number
- The **`Math.random()`** function returns a floating-point, pseudo-random number that's greater than or equal to 0 and less than 1

```js
// Random number from 1-6
Math.trunc (Math.random() * 6) + 1
// Random number from min-max
Math.trunc (Math.random() * (max - min) + 1) + min
```

#### 2. Round integers

```js
Math.trunc()
//Remove decimal parts
Math.round()
//Round to the nearest integer
Math.floor()
//Round down a float to a nearest integer
Math.ceil()
//Round up a float to a nearest integer 
(2.345).toFixed(2)
//return '2.35' (a string)
```

#### 3. Absolute value of a negative number

```JS
Math.abs( )
```

#### 4. Root

```js
Math.sqrt(25)
//return 5
//similar to "25 ** (1 / 2)"
(8 ** (1 / 3))
//return 2
//to get the cubic root
```

#### 5. Min & Max

```js
Math.max(3, 8, 6)
//get the maximum number
Math.min(3, 8, 6)
//get the minimum number
```

#### 6. PI

```js
Math.PI * Number.parseFloat('10px') ** 2
//get the area of a circle with the specified radius
```

#### 7. Even/ Odd

```js
//Check if a number is an Even number
//To repeat sth every N time
const isEven = n => n % 2 === 0
```