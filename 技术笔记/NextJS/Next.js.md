---
title: Next.js
tags: Front-End/NextJS   
started: 2022-11-29 Tue
due: 
modified: 2023-03-01 Wed
status: 
---
## Reference
- Official website: [Next.js by Vercel - The React Framework](https://nextjs.org/)
- Official Tutorials: [Introduction | Learn Next.js](https://nextjs.org/learn/foundations/about-nextjs)
- Official website in Chinese: [Next.js - React 应用开发框架 | Next.js中文网](https://www.nextjs.cn/)
- Next.js 13 Anouncement (Oct 26, 2022) [Blog - Next.js 13 | Next.js](https://nextjs.org/blog/next-13)
- Turbopack Intro [Introducing Turbopack: Rust-based successor to Webpack – Vercel](https://vercel.com/blog/turbopack)
### Videos
- [Next.js 13… this changes everything - YouTube](https://www.youtube.com/watch?v=_w0Ikk4JY7U)
## How to Set Up?
[[How to start a React, NextJS and TailwindCSS project]]
## What?
- Next.js is a popular, lightweight framework for **static and server‑rendered applications**❓ built with React. It comes pre-packaged with features like routing, styling, and server-side rendering, getting your project up and running quickly.
### Different Satges  
- The environment **where** your code runs: **Development vs. Production**
- **When** your code runs: **Build Time vs. Runtime**
- **Where** rendering happens: **Client vs. Server**
### Building Blocks of a Web Application
There are a few things you need to consider when building modern applications. Such as:
- **User Interface** - how users will consume and interact with your application.
- **Routing** - how users navigate between different parts of your application.
- **Data Fetching** - where your data lives and how to get it.
- **Rendering** - when and where you render static or dynamic content.
- **Integrations** - what third-party services you use (CMS, auth, payments, etc) and how you connect to them.
- **Infrastructure** - where you deploy, store, and run your application code (Serverless, CDN, Edge, etc).
- **Performance** - how to optimize your application for end-users.
- **Scalability** - how your application adapts as your team, data, and traffic grow.
- **Developer Experience** - your team’s experience building and maintaining your application.  
For each part of your application, you will need to decide whether you will build a solution yourself or use other tools such as libraries and frameworks.
## Why Next.js?
- Only with React, developers need to spend time **configuring tools and reinventing solutions** for common application requirements.
- Next.js is what you would almost call the **official React framework** 
- Ecosystem friendly
	- out-of-the-box support for TS, JSX, CSS and more
- It also uses SWC same as Vite based on Rust which is faster than Babel as a **compiler**
	- 10x Faster than Vite
	- 700x Faster updates than Webpack (Plugins)
- A new **build tool** - Turbopack built in Rust
- It's faster than Create-React-App
	- 4x faster cold starts than Webpack
- New routing system
	- Easily fetch data for your entire layout
	- Use a new app directory using **file system based routing** like before, but now it's also **directory based**
	- To creat a page, you give the directory the name of the route, then create a `page.js` file to it that exports the component you want to display there.
		- We can co-locate extra components in that directory as well instead of needing to create a separate component directory
	- It opens the door to layouts and nested routing - When you create a `layout.js`, it creates a UI that can be **inherited** by the child routes
		- When navigate to a route inside of a layout, only the inner UI is rendered as opposed to the entire page.
	- Also it has file naming conventions for **loading** and **error** that can render a different UI **at the component level** based on its current state.
		- If a component breaks, it'll render `error.js` instead of `page.js`. The rest of the UI stays intact.
- The most epic feature - Data Fetching
	- All components are React server components by default. **Server components** are a low level primitive in React that **enables SSR**, but until Next.js 13, they've always been difficult for common developer to use.
		- Now we can totally get rid of things like `getStaticProps`, and `getServerSideProps` , instead we can write a plain JS function uses `fetch` (`async function...await`) and `await` the result of that function directly in a component, no need to pass props back and forth between client and server.
		- ![[Pasted image 20230227195806.png]]
- next/image: optimize images on demand
- next/font: custom typefaces for your brand
- next/link: increase your engagement rate
- Vercel 0G Image Generation
- Streaming support - support for HTML streaming, now on Vercel.
- Supports **ISR, SSR, SSG** - the new mental model revolves entirely around caching
### Downsides
- Many features are inspired by Remix. One thing Next is missing is a way to write data similar to Remix forms. 
- There's no way to write **API routes** in the new app directory which seems like a <u>sloppy loose end</u>, as **data fetching** looks amazing but **mutations** are an entirely different story on which the team says they are working on a new **RFC** for mutating data.
- Currently, you would use a client-side component `"use client"` , write your mutation logic and then pass in a callback function of `refresh` to update any data on that route after the mutation is complete, which is similar to React query `useRouter().refresh`
- Major changes- hard to migrate code
- 90 KB baseline of client-side JS (just for warm-up)
	- Other framework that can ship 0 JS app: Astro, Quick
## Rendering Methods
view-source: https://...
#### 1. CSR
- CSR-Client Side Rendering 客户端渲染
#### 2. SSG
- SSG-Static Site Generation 静态页面生成
- By default, all pages will be cached to provide the performance of a static site 
#### 3. SSR
- SSR-Server Side Rendering 服务端渲染
- But if you want new data on every request like SSR, you can add `{cache: 'no-store'}` option to fetch, or for ISR , use the `{next:{revalidate:420}}` option with the number of revalidate seconds. 
- Good for SEO
#### 4. ISR
- ISR-Incremental Static Regeneration 增量静态重生成
- The UI can be incrementally streamed in thanks to React suspense. Just need to define a `loading.js` file to define the UI. If a component is still awaiting data, it'll automatically show it at the component level, while rendering everything else in the application.
## Concepts
### Get Sanity Data in Next.js
#### 1. Libraries needed to get data

```jsx
// Libraries needed to get data
import type { NextPage } from "next";
import Head from "next/head";
import Image from "next/image";
import Link from "next/link";
import { useRouter } from "next/router";

// Sanity Library From Medium-Clone
import { sanityClient, urlFor } from "../sanity"; 

// Sanity Library From Tutorials
import { getClient, usePreviewSubscription } from "@lib/sanity";
import { groq } from "next-sanity";
```

#### 2. Functions used to get data
- getStaticProps
- useRouter
- usePreviewSubscription
- const query = groq`...`
- getClient().fetch()
- sanityClient.fetch()

原理、功能、组件/库  
[https://nextjs.org/blog/next-13](https://nextjs.org/blog/next-13) (Oct 26, 2022)
#### 3. Front-End Framework, Tools/ 前后端初始化方案
- 前端：React, Next.js, TypeScript, 
- 样式：TailwindCSS
- 后端：Sanity
- 基础：HTML, CSS, JS
- 开发工具：
	- prettier
	- eslint
	- react-code-snippets