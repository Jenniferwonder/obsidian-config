---
title: String
tags: Coding/JS
started: 2022-12-01 Thu
due:
modified: 2022-12-06 Tue
status:
number headings: auto, first-level 4, max 6, 1._.1.1.
---
>[Useful string methods - Learn web development | MDN](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Useful_string_methods)
>
## String Format
- Template literals (模板字面量/字符串) `I'm ${firstName}`  
- Multiple lines  
	- `\n\`  
	- `hit enter  
## String Concatenation
#### 1. How to join strings?
- Use [[Operators]] :  `+=`

```js
if (guessCount === 1) {
	guesses.textContent = `Previous guesses: `;
}
guesses.textContent += ` ${guess}`;
```

## String Methods
#### 1. Case Matter

```js
.toLowerCase() 
.toUpperCase()
```

#### 2. Remove white space or new line in a string

```js
.trim()
```

#### 3. Replace

```js
.replace(`original`, `new`)
.replace(/`original`/g, `new`)
//to replace all the same content
```

#### 4. Check if elements in a string

```js
.includes( )
.startsWith( ) 
.endsWith( )
```

#### 5. Split, Join and Add symbols

```js
.split('divider')
//to split the string by a divider in the string
.join(' ')
//to join split strings with a specified divider to one string
.padStart(20, '+') 
.padEnd
//to add symbols to a string to a certain length
```

#### 6. Repeat a String

```js
.repeat(5)
//to repeat the string 5 times
```

#### 7. Convert Number to String
- [[Data Types and Data Structures#Type Conversion and Coersion]]