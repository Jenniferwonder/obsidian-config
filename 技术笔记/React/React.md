---
title: React
tags: Front-End/React    
started: 2022-11-29 Tue
due: 
modified: 2023-01-31 Tue
status: 
---
## Why React?
- ~~What do you know about React?~~
- ~~What is React?~~
- Why do you want to learn and use React?
## How to be good at React?
#### 1. Tools
- [Online Converter-HTML to JSX](https://transform.tools/html-to-jsx)
#### 2. Reference
- New- [Start a New React Project • React](https://beta.reactjs.org/learn/start-a-new-react-project#)
- Old- [Getting Started – React](https://reactjs.org/docs/getting-started.html) 
#### 3. Tutorials
- [Online Courses - Learn Anything, On Your Schedule | Udemy](https://www.udemy.com/course/react-front-to-back-2022/learn/lecture/29767718#reviews)
- [React Website Tutorial for Beginners | Responsive React Website Using Styled Components - YouTube](https://www.youtube.com/watch?v=9_s_Essow6s&list=PLj-4DlPRT48nfYgDK00oTjlDF4O0ZZyG8&index=16)
#### 4. Speech
- [[JSConfUS 2013] Tom Occhino and Jordan Walke: JS Apps at Facebook - YouTube](https://www.youtube.com/watch?v=GW0rj4sNH2w&t=12s)
## React Projects
- [[React Projects]]
## How to start a new React project?
- For learning/ building a SPA (Single Page Application) with React?
	- [Create React App](https://create-react-app.dev/)
	- [Vite](https://vitejs.dev/guide/)
	- [Parcel](https://parceljs.org/getting-started/webapp/)
- For starting a static and server-rendered applications
	- [Next.js](https://nextjs.org/)
- Editor Setup
	- [[VSCode#React Extensions]]
## Core Concepts
### Basics
#### 1. JSX
#### 2. Components
#### 3. Props (proptypes, defaultprops, etc)
#### 4. [[Managing State]] (Component & App Level)
- [Choosing the State Structure • React](https://beta.reactjs.org/learn/choosing-the-state-structure)
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
#### 5. Hooks
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