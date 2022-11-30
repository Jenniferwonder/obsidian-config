---
title: JS-Data Types
tags: JS
started: 2022-11-30 Wed
due: 
modified: 2022-11-30 Wed
status: 
---
## Primitive Data Type
- Number  
- String  
	- Template literals `I'm ${firstName}`  
	- Multiple lines  
		- `\n\`  
		- `hit enter  
- Boolean  
- Undefined  
- Null  
- NaN  
	- not a number  
- Infinity: 23 / 0  
- Symbol(ES2015)  
- BigInt(ES2020)  
	- The biggest number: `2 ** 53 - 1`  
	- Numbers are represented as 64 bits  
	- Only 53 bits are used in JS to store the digits; the rest are used to store decimals  
## Reference Type
- Function  
- Object literals (ES6)  
- Array
- String
- Map (ES6)
- Set (ES6)
- ...
## Type Function
- typeof
### Type conversion
- BigInt( )  
	- hugeNumber+ n  
	- convert a number into big int
- Number()  
	- convert a string to number  
- STring()  
	- convert a number to string  
- Boolean()  
	- Falsy value  
		- 0  
		- ''  
		- undefined  
		- null  
		- NaN  
### Type coersion
## Variable
- Variable: Dynamic Data Type
- Value: Static Data Type
#### Three ways to declare variables
- let
	- Only needed when create a variable for the first time
- const
	- By default
	- Unable to change the value
- var
	- Old

## JS Docs
- jsdoc.app