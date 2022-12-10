---
title: Call Stack and Event Loop
tags: JS   
started: 2022-12-08 Thu
due: 
modified: 2022-12-08 Thu
status: 
---
>[What the heck is the event loop anyway? | Philip Roberts | JSConf EU - YouTube](https://www.youtube.com/watch?v=8aGhZQkoFbQ)

## What is JavaScript?
- A **single-threaded** non-blocking asynchronous concurrent language.
- 单线程、无阻塞、异步、并发
- Have **a call stack**, an event loop, a callback queue and other APIs...
- 调用栈、堆栈溢出（stack overflow）、回调队列/任务队列（回调函数）、事件循环、
### V8
- A JS runtime
- Have a callstack and a heap
![[Pasted image 20221208182251.png]]
## Call Stack
## Blocking?
The V8 can do one thing at a time, but not the browser which can access other APIs.
## Concurrency & Event Loop
call stack > webapis > callback queue > 🔁event loop > task in callback queue? push task to the end of stack
render queue：重绘
