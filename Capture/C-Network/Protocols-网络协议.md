---
Title: Protocols-网络协议
tags: TechSkills
Topic: Protocols
DateStarted: 2023-03-06
DateModified: 2023-05-16
DateDue: 
Total: 0
Completed: 0
Incomplete: 0
status:
sr-due: 2023-07-02
sr-interval: 4
sr-ease: 282
---
## Overview
### Reference
#### 1. Protocols Basics
- [Web性能权威指南 (豆瓣)](https://book.douban.com/subject/25856314/)
	- *High Performance Browser Networking* 本书是谷歌公司高性能团队核心成员的权威之作，堪称**实战经验与规范解读完美结合的产物**。本书目标是涵盖 Web 开发者技术体系中应该掌握的所有**网络及性能优化**知识。全书以性能优化为主线，从 TCP、UDP 和 TLS 协议讲起，解释了如何针对这几种协议和基础设施来优化应用。然后深入探讨了无线和移动网络的工作机制。最后，揭示了 HTTP 协议的底层细节，同时详细介绍了 HTTP 2.0、 XHR、SSE、WebSocket、WebRTC 和 DataChannel 等现代浏览器新增的能力。
#### 2. HTTP/2
> [HTTP/2 - Wikipedia](https://en.wikipedia.org/wiki/HTTP/2) 也是 HTTP 的一个新的协议，于 2015 年被批准通过，现在基本上所有的主流浏览器都默认启用这个协议。所以，你有必要学习一下这个协议
- [http2 explained - The HTTP/2 book](https://daniel.haxx.se/http2/)
- [HTTP2\_White\_Paper\_v4.pdf](https://www.nginx.com/wp-content/uploads/2015/09/NGINX_HTTP2_White_Paper_v4.pdf)
- HTTP/2 的两个 RFC：
	- [RFC 7540 - Hypertext Transfer Protocol Version 2 (HTTP/2)](https://httpwg.org/specs/rfc7540.html) 
		- HTTP/2 的协议本身
	- [RFC 7541 - HPACK: Header Compression for HTTP/2](https://httpwg.org/specs/rfc7541.html)
		- HTTP/2 的压缩算法
#### 3. Web Socket
>新的 HTML5 支持 [WebSocket - Wikipedia](https://en.wikipedia.org/wiki/WebSocket)，所以，这也是你要学的一个重要协议。
- [WebSocket官方文档翻译——HTML5 Web Sockets:A Quantum Leap in Scalability for the Web\_丨知耻而后勇丨的博客-CSDN博客](https://blog.csdn.net/u013252773/article/details/24228375)
	- [Taking a Quantum Leap with Html 5 WebSocket](https://www.slideshare.net/velvetflair/taking-a-quantum-leap-with-html-5-websocket)
	- 这篇文章比较了 HTTP 的几种链接方式，Polling、Long Polling 和 Streaming，并引入了终级解决方案 WebSocket。你知道的，了解一个技术的缘由是非常重要的。
- [javascript - My Understanding of HTTP Polling, Long Polling, HTTP Streaming and WebSockets - Stack Overflow](https://stackoverflow.com/questions/12555043/my-understanding-of-http-polling-long-polling-http-streaming-and-websockets)
	- 这是 StackOverflow 上的一个 HTTP 各种链接方式的比较，也可以让你有所认识。
- [How to WebSockets [Complete Guide] | Treehouse Blog]( https://blog.teamtreehouse.com/an-introduction-to-websockets )
	- 一个 WebSocket 的简单教程。
- [GitHub - facundofarias/awesome-websockets: A curated list of Websocket libraries and resources.](https://github.com/facundofarias/awesome-websockets)
	- GitHub 的 Awesome 资源列表。
- 一些和 WebSocket 相关的想法，可以开阔你的思路
	- [Introducing WebSockets - Bringing Sockets to the Web](https://web.dev/websockets-basics/)
	- [Websockets 101 | Armin Ronacher's Thoughts and Writings](https://lucumr.pocoo.org/2012/9/24/websockets-101/)
	- [The State of Real-Time Web in 2016 - by Paul Banks](https://banksco.de/p/state-of-realtime-web-2016.html)
	- [WebSockets, caution required!](https://samsaffron.com/archive/2015/12/29/websockets-caution-required)
### Resources
### Others

> [Protocol - MDN Web Docs Glossary: Definitions of Web-related terms | MDN](https://developer.mozilla.org/en-US/docs/Glossary/Protocol)

#### 1. [[TCP-IP]]

- Network layers and TCP/IP

#### 2. [[HTTP]]/ [[HTTPS-HTTPS2]]/ [[DNS]]

#### 3. IP/ ICMP

#### 4. TCP/UDP

#### 5. ARP/ RARP
## Related
[[Web, Network, Internet]]