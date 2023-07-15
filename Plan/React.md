---
Title: React
Type: Plan
tags: TechSkills
DateStarted: 2022-11-29
DateModified: 2023-05-16
status:
DateDo:
DateDue: 
DateDone:
Total: 2
Completed: 2
Incomplete: 0
---
## Metadata
- Up:: [[Front-End Frameworks]]
- Jumps:: [[Vue]]
## Purpose
## Scope

## Reference
#### 1. React 入门
- [Tutorial: Tic-Tac-Toe – React](https://react.dev/learn/tutorial-tic-tac-toe)
	- React 学起来并不复杂，就看 React 官方教程和其文档就好了
- React. js 的基本原理
	- [All the fundamental React.js concepts, jammed into this one article](https://www.freecodecamp.org/news/all-the-fundamental-react-js-concepts-jammed-into-this-single-medium-article-c83f9b53eac2)
		- 这篇文章讲了所有的 React. js 的基本原理
	- [Learn React Fundamentals 🆓 and Advanced Patterns ⚛️ 🎁](https://kentcdodds.com/blog/learn-react-fundamentals-and-advanced-patterns)
		- 这篇文章中有几个短视频，每个视频不超过 5 分钟，是学习 React 的一个很不错的地方。
	- [Thinking in React – React](https://react.dev/learn/thinking-in-react)
		- 这篇文章将引导你完成使用 React 构建可搜索产品数据表的思考过程。
#### 2. React 提高
>学习一个技术最重要的是要学到其中的思想和方法。下面是一些我觉得学习 React 中最重要的东西。
##### State-状态
>对于富客户端来说是非常麻烦也是坑最多的地方，这里有几篇文章你可以一读。
- [Common React.js mistakes: Unneeded state - React Kung Fu](https://reactkungfu.com/2015/09/common-react-dot-js-mistakes-unneeded-state/)
	- React.js 编程的常见错误——不必要的状态。
- [State is an antipattern : r/reactjs](https://www.reddit.com/r/reactjs/comments/3bjdoe/state_is_an_antipattern/)
	- 关于如何做一个不错的组件的思考，很有帮助。
- *Why Local Component State is a Trap* 
	- 一些关于 “Single state tree” 的想法。
- [Thinking Statefully](https://daveceddia.com/thinking-statefully/)
	- 几个很不错的例子让你对声明式有状态的技术有更好的理解。
- 传统上，解决 React 的状态问题一般用 Redux。
	- [Tips to learn React + Redux in 2019](https://www.robinwieruch.de/tips-to-learn-react-redux/)
	- Redux 是一个状态粘合组件，一般来说，我们会用 Redux 来做一些**数据状态和其上层 Component 上的同步**。这篇教程很不错。
- *State Architecture Patterns in React* 系列文章，非常值得一读
	- [State Architecture Patterns in React: A Review | by Skyler Nelson | Medium](https://medium.com/@skylernelson_64801/state-architecture-patterns-in-react-a-review-df02c1e193c6)
	- [State Architecture Patterns in React, Part 2: The Top-Heavy Architecture, Flux and Performance | by Skyler Nelson | Medium](https://medium.com/@skylernelson_64801/state-architecture-patterns-in-react-part-2-the-top-heavy-architecture-flux-and-performance-a388b928ce89)
	- [State Architecture Patterns in React, Part 3: Articulation Points, react-zine, An Overall Strategy and Flux-duality | by Skyler Nelson | Medium](https://medium.com/@skylernelson_64801/state-architecture-patterns-in-react-part-3-articulation-points-zine-and-an-overall-strategy-cf076f906391)
##### Functional Programming-函数式编程
>从 jQuery 过来的同学一定非常不习惯 React，而从 Java 等后端过来的程序员就会很习惯了。所以，我觉得 React 就是后端人员开发的，或者说是做函数式编程的人开发的。对此，你需要学习一下 JavaScript 函数式编程的东西。
- 免费电子书
	-  [GitHub - MostlyAdequate/mostly-adequate-guide: Mostly adequate guide to FP (in javascript)](https://github.com/MostlyAdequate/mostly-adequate-guide)
		- [Introduction · JavaScript Functional Programming 指南](https://jigsawye.gitbooks.io/mostly-adequate-guide/content/)
- 前两篇和函数式编程有关的文章非常值得一读。后三篇是一些比较实用的函数式编程和 React 结合的文章。
	- [Master the JavaScript Interview: What is Functional Programming? | by Eric Elliott | JavaScript Scene | Medium](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-functional-programming-7f218c68b3a0)
	- [The Rise and Fall and Rise of Functional Programming (Composing Software) | by Eric Elliott | JavaScript Scene | Medium](https://medium.com/javascript-scene/the-rise-and-fall-and-rise-of-functional-programming-composable-software-c2d91b424c8c)
	- [Functional UI and Components as Higher Order Functions - RisingStack Engineering](https://blog.risingstack.com/functional-ui-and-components-as-higher-order-functions/)
	- [Functional JS Apps: Reverse-engineering the Hype](http://banderson.github.io/functional-js-reverse-engineering-the-hype/#/)
	- [Some Thoughts on Function Components in React | by A. Sharif | JavaScript Inside | Medium](https://medium.com/javascript-inside/some-thoughts-on-function-components-in-react-cb2938686bc7)
##### React 设计模式
- [React Patterns](https://reactpatterns.com/)
	- 一个不错的学习 React 模式的地方
- 如下的一些不错的文章也会对你很有帮助
	- [React Higher Order Components in depth | by franleplant | Medium](https://medium.com/@franleplant/react-higher-order-components-in-depth-cf9032ee6c3e)
	- [Presentational and Container Components | by Dan Abramov | Medium](https://medium.com/@dan_abramov/smart-and-dumb-components-7ca2f9a7c7d0)
	- [Controlled and uncontrolled form inputs in React don't have to be complicated - Gosha Spark](https://goshacmd.com/controlled-vs-uncontrolled-inputs-react/)
	- [Function as Child Components. I recently polled on Twitter regarding… | by Merrick Christensen | Merrick Christensen | Medium](https://medium.com/merrickchristensen/function-as-child-components-5f3920a9ace9)
	
	- [Writing Scalable React Apps with the Component Folder Pattern | by Donavon West | 💅 styled-components | Medium](https://medium.com/styled-components/component-folder-pattern-ee42df37ec68)
	- [Reusable Web Application Strategies: three patterns for running the same app in multiple spots](https://www.freecodecamp.org/news/reusable-web-application-strategies-d51517ea68c8)
	- [Characteristics of an Ideal React Architecture | by Robert Concepción III | Medium](https://medium.com/@robftw/characteristics-of-an-ideal-react-architecture-883b9b92be0b)
##### Best Practice 实践经验
- [9 things every React.js beginner should know - Cam Jackson](https://camjackson.net/post/9-things-every-reactjs-beginner-should-know)
- [Best practices for building large React applications - Sift Engineering Blog : Sift Engineering Blog](https://engineering.sift.com/best-practices-for-building-large-react-applications/)
- [Clean Code vs. Dirty Code: React Best Practices - American Express Technology](https://americanexpress.io/clean-code-dirty-code/)
- [How to become a more productive React Developer - DEV Community](https://dev.to/jakoblind/how-to-become-a-more-productive-react-developer)
- [8 Key React Component Decisions](https://www.freecodecamp.org/news/8-key-react-component-decisions-cc965db11594)
#### Resources
- [GitHub - enaqx/awesome-react: A collection of awesome things regarding React ecosystem](https://github.com/enaqx/awesome-react)
- [GitHub - markerikson/react-redux-links: Curated tutorial and resource links I've collected on React, Redux, ES6, and more](https://github.com/markerikson/react-redux-links)
- 
## Why React?

- ~~What do you know about React?~~
- ~~What is React?~~
- Why do you want to learn and use React?
- ![[zz-assets/Pasted image 20230308093733.png]]

## Error handling

- [React 报错之 Objects are not valid as a React child - chuckQu - 博客园](https://www.cnblogs.com/chuckQu/p/16552571.html)

## How to be good at React?

#### 1. Install [[VS Code]] Extensions for React

#### 2. Tools

- [Online Converter-HTML to JSX](https://transform.tools/html-to-jsx)

#### 3. Reference

- New- [Start a New React Project • React](https://beta.reactjs.org/learn/start-a-new-react-project#)
- Old- [Getting DateStarted – React](https://reactjs.org/docs/getting-DateStarted.html)

#### 4. React Hooks

- [GitHub - alibaba/hooks: A high-quality & reliable React Hooks library.](https://github.com/alibaba/hooks)

#### 5. React Component Libraries

- [[UI Componenet Library]]
- [GitHub - brillout/awesome-react-components: Curated List of React Components & Libraries.](https://github.com/brillout/awesome-react-components#ui-frameworks)
- MUI: [GitHub - mui/material-ui: MUI Core: Ready-to-use foundational React components, free forever. It includes Material UI, which implements Google's Material Design.](https://github.com/mui/material-ui)
- Ant Design: [GitHub - ant-design/ant-design: An enterprise-class UI design language and React UI library](https://github.com/ant-design/ant-design)

#### 6. Tutorials

- [Online Courses - Learn Anything, On Your Schedule | Udemy](https://www.udemy.com/course/react-front-to-back-2022/learn/lecture/29767718#reviews)
- [React Website Tutorial for Beginners | Responsive React Website Using Styled Components - YouTube](https://www.youtube.com/watch?v=9_s_Essow6s&list=PLj-4DlPRT48nfYgDK00oTjlDF4O0ZZyG8&index=16)

#### 7. Speech

- [[JSConfUS 2013] Tom Occhino and Jordan Walke: JS Apps at Facebook - YouTube](https://www.youtube.com/watch?v=GW0rj4sNH2w&t=12s)

## React Projects

- [[React Projects]]

## How to start a new React project?

- For learning/ building a SPA (Single Page Application) with React?
  - [Create React App](https://create-react-app.dev/)
  - [Vite](https://vitejs.dev/guide/)
  - [Parcel](https://parceljs.org/getting-DateStarted/webapp/)
- For starting a static and server-rendered applications
  - [Next.js](https://nextjs.org/)
- Editor Setup
  - [[VS Code#React Extensions]]
- Other Tools/ Frameworks
  - [Storybook: Frontend workshop for UI development](https://storybook.js.org/)
  - [The Fastest Frontend for the Headless Web | Gatsby](https://www.gatsbyjs.com/)

## How to build reusable components?

- [x] Archive/ Timeline
- [x] Dynamic visitor data and feedback
  - Cumulative Page Views 65265  | Unique Visitors 37316
- How to use React Component, Hooks?
- [[UI Componenet Library]]
- React 组件化和 hooks 封装 (复用)

## Core Concepts

![[Pasted image 20230310120115.png]]

### Testing

- [[Testing]]

### Basics

#### 1. JSX

#### 2. Components

#### 3. Props (proptypes, defaultprops, etc)

#### 4. [[Managing State]] (Component & App Level)

- [[Tic-Tac-Toe]]
- button-click/ sync-input
- pic-bg (picture background)
- edit-profile
- letter-highlight
- letter-select

#### 5. Lists & Keys

#### 6. Lifecycle Methods

### Advanced Concepts

#### 1. Styling

#### 2. Form Handling

#### 3. Data Handling

#### 4. Reconciliation Process

#### 5. Hooks (useEffect)

- [A complete guide to the useEffect React Hook - LogRocket Blog](https://blog.logrocket.com/useeffect-hook-complete-guide/)

#### 6. Custom Hooks

#### 7. Context API

### Mastering React

#### 1. Lazy Loading

#### 2. Portals

#### 3. State Management

#### 4. Routing

#### 5. Theming

#### 6. Patterns

#### 7. Anti-Patterns

## Intro
React, a JS library for building UIs.  
Developed at Facebook and released in 2013, **it's safe to say that** React has been the most influential UI library in recent memory [Fireship-as of 2020].  
We use it to build components that represent the logical and reusable parts of the UI.  
The beauty of React is that the simplicity of building a component has been brought down to its theoretical minimum. It's just a JS function.  
The return value from this function is the HTML or UI which is **written** in a special syntax called `JSX`, allowing you to easily combined JS with HTML markup.  
If you wanna pass data into a component, you simply pass in a `prop` argument which you can reference inside the function body or in the UI using braces. If the value changes, React will react to update the UI. (React reacts to changes)  
If we want to give our components its internal state, we can use the `useState` hook.  
The hook is just a function that returns a value as well as a function to change the value.  
![[Pasted image 20230109205028.png|300]]

## Actions

```dataview
TABLE title, DateStarted, status
WHERE contains(title, "React")
SORT file.cday DESC
```
