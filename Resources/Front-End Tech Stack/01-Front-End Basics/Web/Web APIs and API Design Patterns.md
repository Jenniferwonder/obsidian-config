---
title: Web APIs and API Design Patterns
tags: Web
started: 2022-12-02 Fri
due:
modified: 2023-03-15 Wed
status:
---
>[Web APIs | MDN](https://developer.mozilla.org/en-US/docs/Web/API)
## Web APIs
![[Pasted image 20230308095141.png]]
## What is an API?
[REST vs RPC vs GraphQL API - How do I pick the right API paradigm? - YouTube](https://www.youtube.com/watch?v=hkXzsB8D_mo)  
Application Program Interface  
Structured request and response
#### 1. Endpoints
The URI/ URL wwere API/Service can be accessed by a client application (eg. browser)
#### 2. Authentication
Some API required authentication to use their service.
## API Patterns
### REST API
![[Pasted image 20230308202339.png]]
- Representational State Transfer
- Architecture style for designing network application
- Rely on a stateless, **client-server** protocol, almost always HTTP
- Use specific HTTP methods and endpoints
- Fetches all or nothing
- Treat server objects as resources that can be created or destroyed.
- Can be used by virtually any programming language
- JSON as the response type of REST APIs
- Good for CRUD 
#### 1. Pros
- Standard method names, arguments and status code
- Utilized HTTP features
- Easy to maintain
#### 2. Cons
- Big payloads
- Multiple HTTP roundtrips (To get the resource and the sub-resource, you have to get each individually, no way to combine the results together)
#### 3. CRUD
- POST
- PUT
- PATCH
- GET
- DELETE
#### 4. NON-CRUD
- Archive
- Deactivate
- Search
- ![[Pasted image 20230315162159.png]]
### RPC APIs
- Has Endpoints for each action
- GET: for read only request
- POST: for the rest
#### 1. Pros
- Easy to understand
- Lightweight payloads
- High performance
#### 2. Cons
- Discovery is difficult
- Limited standardization
- Leads to function explosion
### GraphQL
- Best when you need querying flexibility
#### 1. Pros
- Save multiple round trips
- Avoid versioning
- Smaller payload size
#### 2. Cons
- Added complexity
- Optimizing performance is difficult
- Too complicated for a simple API  
![[Pasted image 20230308202117.png]]  
![[Pasted image 20230308202453.png]]
## Resources
[[API Resources]]