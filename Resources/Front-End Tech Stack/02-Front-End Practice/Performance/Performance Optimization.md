---
Title: Performance Optimization
tags: Codespace
DateStarted: 2022-12-16
due: null
DateModified: 2023-03-01
status: null
Progress: NaN%
---

## Criteria

![[zz-assets/Pasted image 20230310120346.png]]

## Monitoring Tools

![[zz-assets/Pasted image 20230310120426.png]]

## 性能优化

- ![[zz-assets/Pasted image 20230310120449.png]]
- ![[zz-assets/Pasted image 20230310120508.png]]
  Source: [企业级实战思路 - 什么是亮点 | 大圣前端进阶指南](https://shengxinjing.cn/react/arch/01.arch.html)

1. 性能指标
2. 更快的加载和执行
3. 交互反馈
4. 骨架屏 ...
5. 用大文件上传来举例
6. 懒加载 & 执行
7. 分批执行
8. 不断地思考如何优化（面试官喜欢的场景）
9. [[SEO]]

![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/58082bb8d51e463291a98012efd26c55~tplv-k3u1fbpfcp-zoom-in-crop-mark:4536:0:0:0.awebp)

### 打包阶段

- [Webpack 优化——将你的构建效率提速翻倍](https://juejin.cn/post/6844903924806189070 "https://juejin.cn/post/6844903924806189070")
- [性能优化篇---Webpack 构建速度优化](https://link.juejin.cn?target=https%3A%2F%2Fsegmentfault.com%2Fa%2F1190000018493260 "https://segmentfault.com/a/1190000018493260")
- [webpack 构建速度与结果优化](https://link.juejin.cn?target=https%3A%2F%2Fhuangxsu.com%2F2018%2F08%2F12%2Fwebpack-optimization%2F "https://huangxsu.com/2018/08/12/webpack-optimization/")
- [让你的 Webpack 起飞—考拉会员后台 Webpack 优化实战](https://link.juejin.cn?target=https%3A%2F%2Fzhuanlan.zhihu.com%2Fp%2F42465502 "https://zhuanlan.zhihu.com/p/42465502")
- [webpack dllPlugin 打包体积和速度优化](https://link.juejin.cn?target=https%3A%2F%2Fzhuanlan.zhihu.com%2Fp%2F39727247 "https://zhuanlan.zhihu.com/p/39727247")
- [使用 webpack4 提升 180%编译速度](https://link.juejin.cn?target=http%3A%2F%2Flouiszhai.github.io%2F2019%2F01%2F04%2Fwebpack4%2F "http://louiszhai.github.io/2019/01/04/webpack4/")
- [Webpack 打包优化之速度篇](https://link.juejin.cn?target=https%3A%2F%2Fwww.jeffjade.com%2F2017%2F08%2F12%2F125-webpack-package-optimization-for-speed%2F "https://www.jeffjade.com/2017/08/12/125-webpack-package-optimization-for-speed/")
- [多进程并行压缩代码](https://link.juejin.cn?target=https%3A%2F%2Fjkfhto.github.io%2F2019-10-17%2Fwebpack%2F%25E5%25A4%259A%25E8%25BF%259B%25E7%25A8%258B%25E5%25B9%25B6%25E8%25A1%258C%25E5%258E%258B%25E7%25BC%25A9%25E4%25BB%25A3%25E7%25A0%2581%2F "https://jkfhto.github.io/2019-10-17/webpack/%E5%A4%9A%E8%BF%9B%E7%A8%8B%E5%B9%B6%E8%A1%8C%E5%8E%8B%E7%BC%A9%E4%BB%A3%E7%A0%81/")
- [Tree-Shaking 性能优化实践 - 原理篇](https://juejin.cn/post/6844903544756109319 "https://juejin.cn/post/6844903544756109319")
- [体积减少 80%！释放 webpack tree-shaking 的真正潜力](https://juejin.cn/post/6844903669100445710 "https://juejin.cn/post/6844903669100445710")
- [你的 Tree-Shaking 并没什么卵用](https://link.juejin.cn?target=https%3A%2F%2Fzhuanlan.zhihu.com%2Fp%2F32831172 "https://zhuanlan.zhihu.com/p/32831172")
- [webpack 如何通过作用域分析消除无用代码](https://link.juejin.cn?target=https%3A%2F%2Fdiverse.space%2F2018%2F05%2Fbetter-tree-shaking-with-scope-analysis "https://diverse.space/2018/05/better-tree-shaking-with-scope-analysis")
- [加速 Webpack-缩小文件搜索范围](https://link.juejin.cn?target=https%3A%2F%2Fimweb.io%2Ftopic%2F5a40551ea192c3b460fce335 "https://imweb.io/topic/5a40551ea192c3b460fce335")
- [Brief introduction to scope hoisting in Webpack](https://link.juejin.cn?target=https%3A%2F%2Fmedium.com%2Fwebpack%2Fbrief-introduction-to-scope-hoisting-in-webpack-8435084c171f "https://medium.com/webpack/brief-introduction-to-scope-hoisting-in-webpack-8435084c171f")
- [通过 Scope Hoisting 优化 Webpack 输出](https://link.juejin.cn?target=https%3A%2F%2Fimweb.io%2Ftopic%2F5a43064fa192c3b460fce360 "https://imweb.io/topic/5a43064fa192c3b460fce360")
- [webpack 的 scope hoisting 是什么？](https://link.juejin.cn?target=https%3A%2F%2Fssshooter.com%2F2019-02-20-webpack-scope-hoisting%2F "https://ssshooter.com/2019-02-20-webpack-scope-hoisting/")
- [webpack 优化之 code splitting](https://link.juejin.cn?target=https%3A%2F%2Fsegmentfault.com%2Fa%2F1190000013000463 "https://segmentfault.com/a/1190000013000463")
- [webpack 4: Code Splitting 和 chunks 切分优化](https://juejin.cn/post/6844903922117820423 "https://juejin.cn/post/6844903922117820423")
- [Webpack 大法之 Code Splitting](https://link.juejin.cn?target=https%3A%2F%2Fzhuanlan.zhihu.com%2Fp%2F26710831 "https://zhuanlan.zhihu.com/p/26710831")
- [Better tree shaking with deep scope analysis](https://link.juejin.cn?target=https%3A%2F%2Fmedium.com%2Fwebpack%2Fbetter-tree-shaking-with-deep-scope-analysis-a0b788c0ce77 "https://medium.com/webpack/better-tree-shaking-with-deep-scope-analysis-a0b788c0ce77")
- [Front-End Performance Checklist 2020](https://link.juejin.cn?target=https%3A%2F%2Fwww.smashingmagazine.com%2F2020%2F01%2Ffront-end-performance-checklist-2020-pdf-pages%2F%23top "https://www.smashingmagazine.com/2020/01/front-end-performance-checklist-2020-pdf-pages/#top")
- [（译）2019 年前端性能优化清单 — 上篇](https://juejin.cn/post/6844903765682683911 "https://juejin.cn/post/6844903765682683911")

### 其它优化

- [网站性能优化实战——从 12.67s 到 1.06s 的故事](https://juejin.cn/post/6844903655330562062 "https://juejin.cn/post/6844903655330562062")
- [浏览器页面资源加载过程与优化](https://juejin.cn/post/6844903545016156174 "https://juejin.cn/post/6844903545016156174")
- [聊聊前端开发中的长列表](https://link.juejin.cn?target=https%3A%2F%2Fzhuanlan.zhihu.com%2Fp%2F26022258 "https://zhuanlan.zhihu.com/p/26022258")
- [再谈前端虚拟列表的实现](https://link.juejin.cn?target=https%3A%2F%2Fzhuanlan.zhihu.com%2Fp%2F34585166 "https://zhuanlan.zhihu.com/p/34585166")
- [浅说虚拟列表的实现原理](https://link.juejin.cn?target=https%3A%2F%2Fgithub.com%2Fdwqs%2Fblog%2Fissues%2F70 "https://github.com/dwqs/blog/issues/70")
- [浏览器 IMG 图片原生懒加载 loading=”lazy”实践指南](https://link.juejin.cn?target=https%3A%2F%2Fwww.zhangxinxu.com%2Fwordpress%2F2019%2F09%2Fnative-img-loading-lazy%2F "https://www.zhangxinxu.com/wordpress/2019/09/native-img-loading-lazy/")
- [用 preload 预加载页面资源](https://juejin.cn/post/6844903562070196237 "https://juejin.cn/post/6844903562070196237")
- [App 内网页启动加速实践：静态资源预加载视角](https://link.juejin.cn?target=https%3A%2F%2Fmp.weixin.qq.com%2Fs%3F__biz%3DMzAwNTAzMjcxNg%3D%3D%26mid%3D2651425811%26idx%3D1%26sn%3Df839230a11fa269021c92b510dec47bc%26chksm%3D80dff270b7a87b66abdf73cf9df18efa3e9594c68ab4ca46ba28eb6d3e832969afad031b48fa%26mpshare%3D1%26scene%3D1%26srcid%3D%26sharer_sharetime%3D1569234865992%26sharer_shareid%3D14157f200c2bbcdb4b651ff5559c60ab%26rd2werd%3D1%23wechat_redirect "https://mp.weixin.qq.com/s?__biz=MzAwNTAzMjcxNg==&mid=2651425811&idx=1&sn=f839230a11fa269021c92b510dec47bc&chksm=80dff270b7a87b66abdf73cf9df18efa3e9594c68ab4ca46ba28eb6d3e832969afad031b48fa&mpshare=1&scene=1&srcid=&sharer_sharetime=1569234865992&sharer_shareid=14157f200c2bbcdb4b651ff5559c60ab&rd2werd=1#wechat_redirect")
- [腾讯 HTTPS 性能优化实践](https://link.juejin.cn?target=https%3A%2F%2Fmp.weixin.qq.com%2Fs%2FV62VYS8KFNKxJxfzMYefrw "https://mp.weixin.qq.com/s/V62VYS8KFNKxJxfzMYefrw")
- [Preload, Prefetch And Priorities in Chrome](https://link.juejin.cn?target=https%3A%2F%2Fmedium.com%2Freloading%2Fpreload-prefetch-and-priorities-in-chrome-776165961bbf "https://medium.com/reloading/preload-prefetch-and-priorities-in-chrome-776165961bbf")
- [Front-End Performance Checklist](https://link.juejin.cn?target=https%3A%2F%2Fgithub.com%2Fthedaviddias%2FFront-End-Performance-Checklist "https://github.com/thedaviddias/Front-End-Performance-Checklist")
- [图片与视频懒加载的详细指南](https://link.juejin.cn?target=https%3A%2F%2Fdevelopers.google.com%2Fweb%2Ffundamentals%2Fperformance%2Flazy-loading-guidance%2Fimages-and-video%2F "https://developers.google.com/web/fundamentals/performance/lazy-loading-guidance/images-and-video/")
- [使用 Intersection Observer 来懒加载图片](https://link.juejin.cn?target=http%3A%2F%2Fdeanhume.com%2Flazy-loading-images-using-intersection-observer%2F "http://deanhume.com/lazy-loading-images-using-intersection-observer/")

### 4.6 前端监控

- [5 分钟撸一个前端性能监控工具](https://juejin.cn/post/6844903662020460552 "https://juejin.cn/post/6844903662020460552")
- [把前端监控做到极致](https://link.juejin.cn?target=https%3A%2F%2Fzhuanlan.zhihu.com%2Fp%2F32262716 "https://zhuanlan.zhihu.com/p/32262716")
- [GMTC 大前端时代前端监控的最佳实践](https://juejin.cn/post/6844903629573324807 "https://juejin.cn/post/6844903629573324807")
- [前端监控和前端埋点方案设计](https://juejin.cn/post/6844903650603565063 "https://juejin.cn/post/6844903650603565063")
- [腾讯 CDC 团队：前端异常监控解决方案](https://link.juejin.cn?target=https%3A%2F%2Fmp.weixin.qq.com%2Fs%2FW0i-Iu6nqkWttsGZ-RmOqw "https://mp.weixin.qq.com/s/W0i-Iu6nqkWttsGZ-RmOqw")
