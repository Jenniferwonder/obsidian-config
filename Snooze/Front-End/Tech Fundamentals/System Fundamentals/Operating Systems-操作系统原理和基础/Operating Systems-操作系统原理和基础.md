---
Type: Note
Title: Operating Systems-操作系统原理和基础
tags: 
- TechSkills
DateStarted: 2023-05-17
DateModified: 2023-07-03
status:
DateDo:
DateDue: 
DateDone:
Total: 0
Completed: 0
Incomplete: 0
sr-due: 2023-07-02
sr-interval: 4
sr-ease: 270
---
## Metadata
- Up:: [[System Fundamentals]]
- Jumps::  [[Distributed System Design-分布式技术架构]], [[Computer System Principles-计算机系统原理]], [[Network]]
- Books:: [[B-OS]]
## Purpose
- 学习操作系统的价值在于
	- 理解程序是怎样被管理的，
	- 操作系统对应用程序提供了怎样的支持，
	- 抽象出怎样的编程接口（比如 POSIX/Win32 API），
	- 性能特性如何（比如控制合理的上下文切换次数），
	- 怎样进行进程间通信（如管道、套接字、内存映射等），以便让不同的软件配合一起运行等。  
- 学习操作系统基础原理的好处是，
	- 这是所有程序运行的**物理世界**，无论上层是像
		- C/C++ 这样编译成机器码的语言，
		- Java 这样有 JVM 做中间层的语言，
		- Python/PHP/Perl/Node.js 这样直接在运行时解释的语言，其在底层都逃离不了操作系统这个物理世界的“物理定律”。
	- 可以让你更能从本质理解各种语言或是技术的**底层原理**。一眼看透本质可以让你**更容易地掌握和使用高阶技术**。
## Scope
进程、进程管理、线程、线程调度、多核的缓存一致性、信号量、物理内存管理、虚拟内存管理、内存分配、文件系统、磁盘管理等。  
### MOCs
%% Begin Waypoint %%
- **[[Operating Systems-操作系统原理和基础]]**

%% End Waypoint %%
## Actions
- 一要仔细观察和探索当前使用的**操作系统**，
- 二要阅读操作系统原理相关的图书，这里推荐三本书：
	- 《UNIX 环境高级编程》
	- 《UNIX 网络编程》
	- 《Windows 核心编程》。
- 三要阅读 API 文档（如 man pages 和 MSDN Library），并编写**调用操作系统功能的程序**。
## Reference Links
[^1]: [06 | 如何才能拥有技术领导力？-极客时间](https://time.geekbang.org/column/article/291)