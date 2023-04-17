---
title: Symbol
tags: Coding/JS
started: 2023-02-15 Wed
due: null
modified: 2023-02-15 Wed
status: null
---
## Reference
- [Symbol - JavaScript | MDN](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Symbol)
- [7. Symbols](https://exploringjs.com/es6/ch_symbols.html)
- [JavaScript Symbols: But Why?. Symbols, the newest JavaScript… | by Thomas Hunter II | intrinsic | Medium](https://medium.com/intrinsic-blog/javascript-symbols-but-why-6b02768f4a5c)
## What is symbol?
一个 symbol 值能作为对象属性的标识符；这是该数据类型仅有的目的;
A symbol is a primitive which cannot be recreated?

In this case a symbols is similar to an object as creating multiple instances will result in values which are not exactly equal. But, a symbol is also a primitive in that it cannot be mutated.
```js
const s1 = Symbol();  
const s2 = Symbol();console.log(s1 === s2); // false
```
