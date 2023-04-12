---
title: JSConfUS 2013-JS Apps at Facebook
tags: Coding/JS    
started: 2023-01-13 Fri
due: 
modified: 2023-04-10 Mon
status: 
---
## Topics
- Have you heard about ...?
## Sources
- [[JSConfUS 2013] Tom Occhino and Jordan Walke: JS Apps at Facebook - YouTube](https://www.youtube.com/watch?v=GW0rj4sNH2w&t=12s)
## Useful Expressions
I'm Tom Occhino and thank you Chris **first of all**.  
And I'm gonna **talk a bit about** how we do JS application development at Facebook.  
We're gonna **do something a little different**. Jordan's actually gonna present and he's ~~gonna~~ introduce some of the technical staff. I'm gonna talk about some of the fluffy shit. I'll get out of the way real quick.  
**First of all**, we **ask ourselves this question** many many times - "How should we structure JS applications?"And **more specifically**, JS applications that run in a web browser.  
We're using Node and doing all that fun stuff too, but I'm more **interested in** UI **side of thing**. So that's what we're gonna talk about **today**.  
There're <u>a lot of</u> JS frameworks that **aimed to** answer this question.  
Um... These frameworks have <u>allowed us</u> to move the web forward as a real application platform.  
**Their consensus** **is basically that** the MVC style architecture is the best. And it's not just MVC, right? It's MVVM or as Angular calls it modal-view whatever. I really like that one.  
I actually really like Angular **in** the declarative data binding. I think that's kind of the **holy grail** **in terms of** the APIs.  
All of these architectures and frameworks **have one thing in common** **though**. And that's "Modals." So **typically**, "modals" in these frameworks implements **observable objects** with an advanced API. Developers use **bi-directional data binding** to bind their views with their modals. **As** their modals changed, their views can be updated. And as theirs views changed, they can update their modals or some properties out of views.  
So this **observable-modal pattern** encourages **mutation** now.  
And **mutation** is complex. So a few years ago, starting with our chat rewrite, we start to structure our application a little differently. We wanna **minimize** some of the mutations developers had to deal with. Mutation is **an necessary evil** you have to **deal with** it. But we wanna minimize the mutations developers have to code themselves.  
So let me **show you what I mean by that**.  
Here's a structure for a simple application. In this diagram **you'll notice that** all updates go through a single flow, so all updates including user input, they all go through a single channel. This is one directional data binding. Those updates **eventually** reach the views. In this simplest way we have found **conceptually** to resturcture and render our views is to just trying to avoid mutation altogether. **What I mean by that** is anytime your data changes it just blow away your view completely and re-render it **from scratch**. Now I know what you're thinking. That's not gonna work right? The DOM can be slow. Browser can be **prohibitively expensive** trying to do this. 
