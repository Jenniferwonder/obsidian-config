---
title: Node.js and Package manager
tags: Coding   
started: 2022-11-29 Tue
due: 
modified: 2023-03-13 Mon
status: 
---

## What is Node?
A JS runtime to run JS in the server  
![[Pasted image 20230310115943.png]]
## Install Node
[Node.js](https://nodejs.org/en/)  
REPL mode - read of all print loop
- `node -v`, to know the version installed
#### 1. How to use NVM (Node version manager)
![[Pasted image 20230301092447.png]]
## How to use Node?
In terminal, 
- type `node`, then it can run JS code.
- type `node .` /`node index.js` to run the `index.js` file
## Understand Runtime
Unique identifiers
- `global` similar to `window` object, value of which can be accessed anywhere
- `process.platform` gives you access to the currently running node process, with which we can check the current platform or OS 
- `process.env.USER` to grab an environment variable from your server
## How do Events work in Node.js?
an asynchronous event-driven JS runtime.  
Event loop - non-blocking  
![[Pasted image 20230301094039.png]]
#### 1. How do Event and Callback work in Node?
- Built-in Event
	- ![[Pasted image 20230301094450.png]]
- Built own event: import `{EventEmitter}` from `events` module built in Node, then create a custom `eventEmitter` by instantiating the class, and register a callback that fires on the `lunch` event, then we can call `eventEmitter.emit('lunch')` which triggers callback function to run.
	- ![[Pasted image 20230301095205.png]]  
This event-driven programming is useful when you have something that is CPU intensive.
## File System
Built-in file system module called `fs`, which can read, write and delete files on the file system among other things, and it can also do things in a blocking or non-blocking way.
#### 1. Eg. Read File
Import two functions from the file system module, called `{readFile, readFileSync}`. Anytime you see a function ends in `sync` think blocking.  
We can read a text file in Node by simply passing the path to that file and we'll specify the encoding as `'utf8'`.
##### 1.1. Blocking
![[Pasted image 20230301100205.png]]
##### 1.2. Non-Blocking
- Tip1: Use Callback
	- ![[Pasted image 20230301100308.png]]
- Tip 2: Use Promise-based solutions
	- Import `readFile` from the `promises` namespace, which gives us a function returning a promise when called
	- ![[Pasted image 20230301100827.png]]
	- ![[Pasted image 20230301100907.png]]
## Modules & NPM
A module is a JS file that exports its code  
Node has a bunch of built in modules
#### 1. How to use Modules?
Tradition way to import a module is to use `require()` function (Common JS). Node also added support for ES modules `import/export`, but most Node.js code written in JS still uses `require()`
##### 1.1. Use modules in our own code base?
- Create a new file `my-module.js` to serve as your module
- Then go to `index.js` file, create a variable for the module, then import it using `require()`
- In the module file, we can reference the object using `module.exports`, we can add properties to the object or redefine it as a new object, which will be available to use in other file
##### 1.2. Use modules created by other people?
- NPM (Node package manager) which was acquired by GitHub which was acquired by Microsoft (2020.5).
- When you intall Node, you also install **NPM** which is a tool you can use to install remote packages to use in your own code.
- To use NPM
	- `npm init -y` using y flag to use the default options, which creates a `package.json` file in the root of the application which contains meta data about your project, and keeps track of the dependencies you use here.
	- `npm install express` to install Express, which is a minimal web application framework
	- The dependency object allows you to manage multiple dependencies in a project and then reinstall them all at once on a different system.
	- The actual raw source code for the dependency lives in this `node_modules` directory which should never be modified, because the `package.json` controls how this directory is built. It fetches your remote packages, saves your source code here, which should be able to be repeated on any system.
	- We can import the package installed by name `const express = require('express')`
## Build and Deploy
Build a full-stack application and deploy it to the cloud.  
Our **Server** will live on a URL. When user makes a request to this URL in the browser, the Server will response with some HTML.
- In our code, we'll first create an instance of an **Express app**, which allows us to <u>create different URLs and endpoints</u> that a user can navigate to in the browser,
- Then we define code in the server to **handle those requests** ("I don't want to get too deep into HTTP"). When the user navigates to a URL inthe browser, it's what's known as a `get` request, meaning they are requesting some data on the server and not trying to modify or update anything.
- With Express, we can set up an endpoint like that by calling `app.get()`, 
	- and then **the first argument** is the **URL** that the user will navigate to. We use a forward slash `/` for the root URL but feel free to create **multiple pages** for  your web app by creating different URLs. 
	- The second argument is our **callback function**. You can think of every request to this URL as an event and then you handle that event with this function.
	- Express gives us two params to make use of, the **request** and **response**.
	- **Request** is the incoming data from the user. In some cases, you might want to look at the **headers** or the **body** of the request to authenticate a user or understand what the user is trying to do. 
	- **Response** is your outgoing data
		- At this point,we need to implement the code to handle the request - reading some HTML from our file system and then send it back down to the browser.
		- ![[Pasted image 20230301110202.png]]
	- Now we have a way to send HTML from the Server to the Client.
- Now we need to tell our Express app to **start listening** to incoming requests.
	- We do that by defining a port which will normally come from `process.env.PORT`, a node environment variable,
	- Then we call `app.listen()` with that port, and when it starts up, we'll `console.log('App available on http://localhost:3000')`
	- You can start it up by opening the command line and running Node with the current working directory `node .`.
	- If you go ahead and open it in the browser, you should see your HTML returned back to you.
- The callback can be very difficult to work with as your app grows in complexity. It often leads to a state known as **callback hell** where. To avoid this, use `promise`.
	- ![[Pasted image 20230301111713.png]]![[Pasted image 20230301111654.png]]
## How to Deploy?
[[Deploying]]
#### 1. Google App Engine 
##### 1.1. What and why?
- (Fully managed serverless application platform) - an easy and free way, 
- It has a standard environment for Node.js
- Provide with a **Server** in the cloud that **scales automatically** based on the incoming traffic to your app
##### 1.2. How to use?
- It's easy to set up but you first need to have a <u>Google cloud platform account</u> and <u>Google command line tools</u> installed.
- Once done, you can go into your source code and create an `app.yaml` file, which is used to configure your cloud server. The only thing we need at this time is to specify a runtime of Node.js version `runtime: nodejs12`
- App engine will run your code by looking in the `package.json` file for a start script `"scripts": {"start": "node ."}`.
- From there, we can open the command line and run `gcloud app deploy`, that'll take a minute and then it will give you a URL where you can access your app publicly on the web.
## Next.js or Express?
>[Build a server-rendered React app with Next.js and Express - LogRocket Blog](https://blog.logrocket.com/build-server-rendered-react-app-next-express/)  
>[javascript - NextJS vs Express - Stack Overflow](https://stackoverflow.com/questions/69918766/nextjs-vs-express)
### ExpressJS vs NextJS features
#### 1. Some ExpressJS features are:
- Robust routing
- HTTP helpers (redirection, caching, etc)
- View system supporting 14+ template engines
#### 2. Next.js provides the following key features:
- Zero setup. Use the filesystem as an API ( You do not need Express to build a full-stack application)
- Server-Side rendering (SSR)
- Static site generation (SSG)
- Single-Page application (SPA)
- Development of faster applications
- Optimization of pages
- SEO websites
- Automatic code splitting
### Conclusion
Express.js is a **backend framework for building APIs** whereas Next.js is a **full stack framework that builds upon React** to improve the SEO, development experience, and performance of your project. One of these features IS a built-in API routing system that **could** replace Express.js.  
It all depends on the case you have and your personal preference. If you are building a private page (admin panel that can only be accessed with authentication) that does not need to be found by search engines, you do not need Next.js and will need Express.js. If you are building a public website (e.g. e-commerce website) and you are using Next.js for SEO optimization, you **could** replace Express.js with it.  
**TLDR;** You can replace an Express API with NextJS's API routing system but that only makes sense if you're building a full-stack React project. If it's a standalone API, using Next.js to replace just that API doesn't make any sense.  
Next.js on its own is a powerful tool. When combined with Express, it makes a sacred combination. Using Express with Next.js, you can:
### Why use Express with [[Next.js]]?
- Easily build web socket features in your applications
- Develop custom or extra logic for your Next.js routes
- Build Express middleware and fetch data for Next.js pages before they are rendered
- Easily build backend features, such as file uploading, media file compression, and more
### Advantages of using Express with Next.js
The great thing about Next.js is that there are a lot of advantages, not only for the developers, but also for the users and business owners using Next.js in the technology stack.  
For developers, Next.js has:
- A growing community of experienced developers and contributors, hence easy adoption by other developers and easy-to-find solutions to any issues you might face while learning and using Next.js
- An automatic feature that helps you optimize images, and has automatic lazy-loading, preloading of critical images, correct sizing across devices, and supports modern formats.
- A faster browser refresh rate while you’re developing
- Out-of-the-box support for TypeScript
- Automatic compilation and bundling so you don’t waste time with a lot of configurations to get your application running
- Easy creation of API routes or endpoints during application development
- Content rendering in multiple ways. You can prerender with server-side rendering or static site generation, or can update or create your application content at runtime with incremental static regeneration  
Some other advantages of using Express with Next.js also include:
- Data security: websites created with Next.js are static and don’t have a direct connection with your application database, user information, third-party integration keys, and any other sensitive information
- Search engine friendliness: because Next.js websites load fast and are easy to scan by search engine bots, this improves organic traffic to the website and can translate to conversions and sales for the owner of the website
- Cross deployment: you can use Next.js to build across several platforms. You can build Static web applications, Progressive Web Apps (PWA), and even mobile apps using Next.js

