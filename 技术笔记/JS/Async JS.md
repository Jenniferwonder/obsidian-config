---
title: Async JS
tags: Front-End/JS  
started: 2022-12-08 Thu
due: 
modified: 2022-12-09 Fri
status: 
---

## What?
>[Asynchronous JavaScript - Learn web development | MDN](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Asynchronous)

## Why?
>[[Event Loop-事件循环]]
1. Start a long-running operation by calling a function.
2. Have that function start the operation and return immediately, so that our program can still be responsive to other events.
3. Notify us with the result of the operation when it eventually completes.
#### 1. Example - Event-loop

```js
// L1
console.log('🥪 Synchronous 1');
// L2
setTimeout(_ => console.log(`🍅 Timeout 2`), 0);
// L3
Promise.resolve().then(_ => console.log('🍍 Promise 3'));
// L4
console.log('🥪 Synchronous 4');
```

## How? -- Three Techniques
- [[Callbacks]]
- [[Promise]]
- [[Async...await]]