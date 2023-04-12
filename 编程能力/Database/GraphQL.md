---
title: GraphQL
tags: Coding   
started: 2023-03-01 Wed
due: 
modified: 2023-03-01 Wed
status: 
---
## Reference
[GraphQL | A query language for your API](https://graphql.org/)  
[GraphQL Explained in 100 Seconds - YouTube](https://www.youtube.com/watch?v=eIQh02xuVw4)  
[GraphQL Basics - Build an app with the SpaceX API - YouTube](https://www.youtube.com/watch?v=7wzR4Ig5pTI)
## What is GraphQL?
A **query language** for reading and mutating data in APIs.  
As a back-end developer, GraphQL provides **a type system** where you can describe **a schema** for your data. In turn, it give front-end consumers of the API the power to **explore and request** the exact data they need.  
Traditionally, web developers have consumed APIs using **REST API**, where **data entities** live on a bunch of URLs on a server. When the request is received, the API responds with the full data payload of that entity. But it has TWO drawbacks:
- We may need multiple entities at one time, in which case each request is **under fetching** the actual data we want;
- We may want a small subset of a data entity, in which case we need to **over fetch** from the API, which is bad for the environment.  
A GraphQL API has a single entry point. Data is queried or fetched by describing it with a syntax that mirrors its return shape in `json`.  
The front-end developer describes the data they want while the back-end developer writes code to resolve the request.  
![[Pasted image 20230301190231.png]]
## How to use?
#### 1. Define a schema
We can start **defining a schema** with our own custom objects using the `type` keyword. 
- A `type` can have multiple fields like a unique `id: ID!` and we'll make that required with a bang `!` , let's also give it interger `int` and `String` values, then create a relationship with another type. 
- A creator can have many videos which we can represent by wrapping the type in brackets `videos:[Video]`. On the flip side, a video belongs to a creator.
	- ![[Pasted image 20230301190845.png]]
- Every GraphQL API has a `type Query` type,  which is a main entry point to **read data**. We can query a list of videos or an individual user based on their id. 
	- ![[Pasted image 20230301191155.png]]
- That's how a consumer reads data but they may also want to **mutate data**, in which case we implement `type Mutation` that defines how data can be modified on the API.
	- ![[Pasted image 20230301191354.png]]
#### 2. Resolve Data
- From there, we can define code to **resolve** this data in any programming language (Resolvers)
	- ![[Pasted image 20230301191523.png]]
- Once deployed, any developer consuming this API will be able to explore it with a complete understanding of **all possible queries and data entities**, which means the tooling can **auto-complete** your query as you type it out in your editor.
	- ![[Pasted image 20230301191929.png]]