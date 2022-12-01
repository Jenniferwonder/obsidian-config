---
title: Data Types
tags: JS
started: 2022-11-30 Wed
due: 
modified: 2022-12-01 Thu
status: 
number headings: auto, first-level 4, max 6, 1._.1.1.
---
## Value and Variable
#### 1. Value
- [[Data Types#Primitive Data Type]]
#### 2. Variable
- Dynamic Data Type
##### 2.1. Three ways to declare variables
```js
let
//Only needed when create a variable for the first time
const
//By default
//Unable to change the value
var
//Old
```
## Primitive Data Type
#### 1. [[Number]]  
#### 2. [[String]]  
#### 3. Boolean  
##### 3.1. Falsy value  
```js
0  
''  
undefined  
null  
NaN  
```
#### 4. Undefined  
#### 5. Null  
#### 6. NaN  
- not a number  
#### 7. Infinity: 23 / 0  
#### 8. Symbol(ES2015)  
#### 9. BigInt(ES2020)  
- The biggest number: `2 ** 53 - 1`  
- Numbers are represented as 64 bits  
- Only 53 bits are used in JS to store the digits; the rest are used to store decimals  
## Reference Type
#### 1. [[Function]]  
#### 2. [[Object]] 
#### 3. [[Array]]
#### 4. Map (ES6)
#### 5. Set (ES6)
#### 6. ...
## Type Conversion and Coersion
#### 1. Check value type
```js
.typeof
```
#### 2. Convertion
```js
//Convert a number into big int
BigInt( )  
//Convert a string to number  
Number()
//Convert a number to string  
String()  
//Convert to boolean
Boolean()  
```
#### 3. Type coersion
```js
+''
//convert a string to number  
```

## JS Docs
- jsdoc.app