---
title: React
tags: Coding/React
started: 2022-11-29 Tue
due:
modified: 2023-03-01 Wed
status:
---
## Why React?
- ~~What do you know about React?~~
- ~~What is React?~~
- Why do you want to learn and use React?
- ![[Pasted image 20230308093733.png]]
## Error handling
- [React报错之Objects are not valid as a React child - chuckQu - 博客园](https://www.cnblogs.com/chuckQu/p/16552571.html)
## How to be good at React?
#### 1. Install [[VS Code]] Extensions for React
#### 2. Tools
- [Online Converter-HTML to JSX](https://transform.tools/html-to-jsx)
#### 3. Reference
- New- [Start a New React Project • React](https://beta.reactjs.org/learn/start-a-new-react-project#)
- Old- [Getting Started – React](https://reactjs.org/docs/getting-started.html) 
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
- [[NextJS-Projects]]
## How to start a new React project?
- For learning/ building a SPA (Single Page Application) with React?
	- [Create React App](https://create-react-app.dev/)
	- [Vite](https://vitejs.dev/guide/)
	- [Parcel](https://parceljs.org/getting-started/webapp/)
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
- [[React]] 组件化和 hooks 封装 (复用)

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
## Logs

```dataview
TABLE title, started, status
WHERE contains(title, "React")
SORT file.cday DESC
```