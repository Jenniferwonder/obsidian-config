---
title: ZTM JS Note
tags: null
status: null
started: null
due: null
aliases: null
---
### Goals
#### JavaScript
- [x] **Basics**: number, string, operands, variables, array, list, object, conditionals, loops（Aug 11）
- [x] **DOM** (Aug 12- )
### Basics
#### Time: 
- Aug 11-
#### Key Concepts:
OutlineJAVASCRIPT TYPES
-----------------
1. Number 
2. String
3. Boolean
4. Undefined
5. Null
<!-- 6. Symbol (new in ECMAScript 6) -->
1. Object
JAVASCRIPT COMPARISONS
-----------------
!==
===

>=
<=
>

<
JAVASCRIPT VARIABLES
-----------------
var
<!-- let (new in ECMAScript 6)-->  
<!-- const (new in ECMAScript 6)-->
JAVASCRIPT CONDITIONALS
-----------------
if
else
else if
<!-- ternary operator -->
<!-- switch -->
JAVASCRIPT LOGICAL OPERATORS
-----------------
&&
||
!
JAVASCRIPT FUNCTIONS
-----------------
var a = function name() {}
function name() {}
return
<!-- () => (new in ECMAScript 6) -->
JAVASCRIPT DATA STRUCTURES
-----------------
Array
Object
JAVASCRIPT LOOPING
-----------------
for
while
do 
forEach (new in ECMAScript 5) 
JAVASCRIPT KEYWORDS
-----------------
break
case
catch
class
const
continue
debugger
default
delete
do
else
export
extends
finally
for
function
if
import
in
instanceof
new
return
super
switch
this
throw
try
typeof
var
void
while
with
yield
DOM SelectorsDOM Selectors
--------------
getElementsByTagName
getElementsByClassName
getElementById
querySelector
querySelectorAll
getAttribute
setAttribute
##Changing Styles
style.{property} //ok
className //best
classList //best
classList.add
classList.remove
classList.toggle
##Bonus
innerHTML //DANGEROUS
parentElement
children
##It is important to CACHE selectors in variables
### Resources
#### Array:
- 
#### DOM Selectors:
- 
- 
#### Event:
- 
- Keyboard Event
   - 
### Tools
Can I use: 
### Practice and enhancement
#### Insights1: How to check for ENTER key press in JavaScript?
❗Avoid Mistakes: 
   - select the wrong element. ie. "~~button~~"
   - missing ";"

```javascript
input.addEventListener("keypress", function(event) {// Keyboard event
    //console.log(event);
    if (input.value.length > 0 && event.key === "Enter") { 
        var li = document.createElement("li");
        li.appendChild(document.createTextNode(input.value));
        ul.appendChild(li);
        input.value = ""; 
    }
});
```

```javascript
document.addEventListener('keydown', (event) => {
    const keyName = event.key;
    if (input.value.length > 0 && keyName === "Enter") { 
        var li = document.createElement("li");
        li.appendChild(document.createTextNode(input.value));
        ul.appendChild(li);
        input.value = ""; 
    }})
```

#### Insight2: How to avoid code repetition?
💡Create "**function"** for repetitive code

```javascript
var button = document.getElementById("enter");
var input = document.getElementById("userinput");
var ul = document.querySelector("ul");
button.addEventListener("click", function() {// Mouse event
    //console.log(input.value);
    if (input.value.length > 0) { /* To avoid adding empty list*/
        var li = document.createElement("li");
        li.appendChild(document.createTextNode(input.value));
        ul.appendChild(li);
        input.value = ""; /* To clear the box after enter */
    }
});
input.addEventListener("keypress", function(event) {// Keyboard event
    console.log(event);
    if (input.value.length > 0 && event.key === "Enter") { 
        var li = document.createElement("li");
        li.appendChild(document.createTextNode(input.value));
        ul.appendChild(li);
        input.value = ""; 
    }
});
```

```javascript
var button = document.getElementById("enter");
var input = document.getElementById("userinput");
var ul = document.querySelector("ul");
function inputLength() {
    return input.value.length;
}
function createListElement() {
    var li = document.createElement("li");
    li.appendChild(document.createTextNode(input.value));
    ul.appendChild(li);
    input.value = ""; /* To clear the box after enter */
}
button.addEventListener("click", function() {// Mouse event
    //console.log(input.value);
    if (inputLength() > 0) { /* To avoid adding empty list*/
        createListElement(); 
    }
});
input.addEventListener("keypress", function(event) {// Keyboard event
    //console.log(event);
    if (inputLength() > 0 && event.key === "Enter") { 
        createListElement(); 
    }
});
```

```javascript
var button = document.getElementById("enter");
var input = document.getElementById("userinput");
var ul = document.querySelector("ul");
function inputLength() {
    return input.value.length;
}
function createListElement() {
    var li = document.createElement("li");
    li.appendChild(document.createTextNode(input.value));
    ul.appendChild(li);
    input.value = ""; /* To clear the box after enter */
}
function addListAfterClick() {// Click event
    if (inputLength() > 0) { /* To avoid adding empty list*/
        createListElement(); 
    }
}
function addListAfterKeypress(event) {// Keyboard event
    //console.log(event);
    if (inputLength() > 0 && event.key === "Enter") { 
        createListElement(); 
    }
}
button.addEventListener("click", addListAfterClick);
input.addEventListener("keypress", addListAfterKeypress);
```