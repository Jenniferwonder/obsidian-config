---
title: Deploying
tags: Front-End    
started: 2022-11-29 Tue
due: 
modified: 2023-03-13 Mon
status: 
---
## Reference

- [大公司里怎样开发和部署前端代码？](https://link.juejin.cn?target=https%3A%2F%2Fwww.zhihu.com%2Fquestion%2F20790576 "https://www.zhihu.com/question/20790576")
- [前端高级进阶：前端部署的发展历程](https://juejin.cn/post/6844904086823780366 "https://juejin.cn/post/6844904086823780366")
## [[CI-CD]] 
- GitHub Actions (Auto Deploy)
- CI- Continuous Integration
- CD- Continuous Development
## Fullstack Deployment
Server-side apps need a server to execute your code
#### 1. PaaS
- Platform as a service
- Everything is set up for you without need to set up a server (Install **Nginx** and firewalls...)
- Only need to push your code to GitHub and select the repo from within the platform much like you do with Netlify
##### 1.1. Render.com
With free tier
##### 1.2. Heroku
Stop free tier since 2022
#### 2. Cloud Hosting
- Unmanaged cloud hosting
- You rent out a Linux box and you can install whatever you want on it any Linux disk draw, any programs you want, set up Nginx and web servers and all that, but that's much more difficult
##### 2.1. Lenode
- You can install the OS, 
- Have to set everything up from scratch; you'll be installing your web servers, node.js or whatever your backend is using
##### 2.2. AWS/ Azure
- Great for large projects with a lot of traffic
- Tons of services
## Questions
- How to deploy a React, Next.js+ Sanity project?
	- Vercel
- 自动化部署 (部署效率) ...
- [[SEO]]
- [[CDN]]
- [[DNS]] 
- [[Security]]
- [[Server]]
- Monitor user traffic
- 图床 