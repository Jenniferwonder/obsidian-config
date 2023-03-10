---
title: Testing
tags: Front-End   
started: 2023-03-01 Wed
due: 
modified: 2023-03-01 Wed
status: 
---
[Test-Driven Development // Fun TDD Introduction with JavaScript - YouTube](https://www.youtube.com/watch?v=Jv2uxzhPFl4)
[如何使用React Testing Library和Jest测试React应用 · Issue #16 · vortesnail/blog · GitHub](https://github.com/vortesnail/blog/issues/16)
## What
![[Pasted image 20230308094955.png]]
## Why Testing?
A well-designed suite of **automation** tests is effective in allowing you to 
- Discover defects or bugs before delivery to the client
- Guarantee the quality of the software you develop further by catching bugs before they find their way into a live application
- Reduce user complaints and save time and money
## Best Practices
- Avoid including implementation details. 
- Final users will have no notion of React. Rather than dealing with instances of rendered React components, your tests should **wok with actual DOM nodes**.
- Resemble software usage
- Maintainability in the long run - as long as you're not changing functionality any changes in the implementation of the component won't break your tests and slow you and your team down

## React Testing Library and Jest
Two tools React endorses to structure your tests.
#### 1. Jest
A JS test runner that lets you access an artificial DOM called jsdom. While jsdom is an approximation of how the browser works, it's often good enough for testing React component.
- Good iteration speed
- Powerful features, like **mocking** modules so you can have more control over how the code executes, to make sure your unit testing is standalone.
#### 2. React Testing Library
A set of **utilities** that let you test React components without relying on their implementation details, designed to fulfill the best practices for us to get a **well-configured testing environment** out of the box and are able to focus on the business logic your tests need to run assertions on.
#### 3. Storybook
#### 4. Mocha
## TDD-Test Drivern Development Philosophy
#### 1. End-To-End
#### 2. Integration
#### 3. Unit

