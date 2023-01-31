---
title: React
tags: React    
started: 2022-11-29 Tue
due: 
modified: 2023-01-30 Mon
status: 
---
## Topics
- What do you know about React?
## 参考资料
### Reference
[Getting Started – React](https://reactjs.org/docs/getting-started.html)  
[Home v6.6.1 | React Router](https://reactrouter.com/en/main)
### Tutorials
### Courses
- [Online Courses - Learn Anything, On Your Schedule | Udemy](https://www.udemy.com/course/react-front-to-back-2022/learn/lecture/29767718#reviews)
- [React Website Tutorial for Beginners | Responsive React Website Using Styled Components - YouTube](https://www.youtube.com/watch?v=9_s_Essow6s&list=PLj-4DlPRT48nfYgDK00oTjlDF4O0ZZyG8&index=16)
### Speech
- [[JSConfUS 2013] Tom Occhino and Jordan Walke: JS Apps at Facebook - YouTube](https://www.youtube.com/watch?v=GW0rj4sNH2w&t=12s)
### Tools/ Resources
## 学习前提
#### 1. [[JavaScript]]
## 项目案例
[[React Projects]]
## 核心知识
### Basics
#### 1. Initializing React
- create react app
- index.html > index.js
	- use `index.js` to insert html into `index.html` `<div id="root"></div>`
- 
#### 2. Components
#### 3. JSX
#### 4. Props (proptypes, defaultprops, etc)
#### 5. State (Component & App Level)
#### 6. Styling
#### 7. Handling Events
#### 8. Lists & Keys
#### 9. Forms
#### 10. Context API
#### 11. HTTP Requests
1. [Understand React](https://reactjs.org/tutorial/tutorial.html#what-is-react)
2. How To Set Up Your DevEnv
3. JSX
4. Components
5. State
6. Props
7. Lists/Keys
8. Lifecycle Methods

### Advanced React Concepts

1. Styling
2. Form Handling
3. Data Handling
4. Reconciliation Process
5. Hooks
6. Custom Hooks
7. Context

### Mastering React

1. Lazy Loading
2. Portals
3. State Management
4. Routing
5. Theming
6. Patterns
7. Anti-Patterns
## Intro
React, a JS library for building UIs.  
Developed at Facebook and released in 2013, it's safe to say that React has been the most influential UI library in recent memory [Fireship-as of 2020].  
We use it to build components that represent the logical and reusable parts of the UI. The beauty of React is that the simplicity of building a component has been brought down to its theoretical minimum. It's just a JS function.  
The return value from this function is the HTML or UI which is written in a special syntax called `JSX`, allowing you to easily combined JS with HTML markup. If you wanna pass data into a component, you simply pass in a `prop` argument which you can reference inside the function body or in the UI using braces. If the value changes, React will react to update the UI. (React reacts to changes)  
If we want to give our components its internal state, we can use the `useState` hook. The hook is just a function that returns a value as well as a function to change the value.  
![[Pasted image 20230109205028.png|300]]