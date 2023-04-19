---
title: System Design Methodology
tags: System-Design
started: 2023-03-13 Mon
due:
modified: 2023-03-15 Wed
status:
---
[System Design for Beginners Course - YouTube](https://www.youtube.com/watch?v=m8Icp_Cid5o)
## Design Patterns
A general **reusable solution** to a commonly occuring problem within a given context in software design.  
Convert business requirements into technical solutions  
![[Pasted image 20230310112005.png]]
#### 1. Publisher-subscriber model
## Reference
[Systems Design Interview Concepts (for software engineers / full-stack web) - YouTube](https://www.youtube.com/watch?v=REB_eGHK_P4)  
[System Design Course for Beginners - YouTube](https://www.youtube.com/watch?v=MbjObHmDbZo)
## Distributed Systems 
#### 1. Intro
#### 2. Performance Metrics
#### 3. Interview Style Example
## Load Balancing
- Balance incoming traffic to multiple servers
- Used to improve reliability and scalability of application
- Software: Nginx, HAProxy
- Hardware: F5, Citrix
#### 1. Load Balancers
![[Pasted image 20230315164956.png]]
#### 2. Routing Methods
- Round Robin
- Least Connections
- Least Response Time
- IP Hash
	- Routes client to server based on IP
	- Useful for stateful sessions
#### 3. L4 VS L7
##### 3.1. Layer 4
- Only has access to TCP and UDP data
- Faster
- Lack of info can lead to uneven traffic
- Good on the edge of your data center or of your network, because it can look at the IP address and if you're getting a denial of service attack or some bad actors going after application, instead of wasting processing power allowing it through to your web server or your application, you can toss that request at the edge, so lots of data centers will first route all incoming traffic through a layer 4 LB(Load balancer)
##### 3.2. Lyer 7
- Full access to HTTP protocol and data
- SSL termination
- Check for authentication
	- If a user sends a request they're not logged in, they're trying to get to a certain page, instead of letting that go to your application server, at the LB you could redirect those people
- Smarter routing options
	- as a result of having access to the entire url of the request and all the data within that, you have a lot of smarter routing options.
- It's more CPU intensive
## Caching
#### 1. What?
When you cache something, you take data that would normally be stored on a hard drive or a disk, you put it into memory.
#### 2. Why?
- Improve speed and performance of your application
	- Reading from memory is 50-200x faster than disk
	- Can serve the same amount of traffic with fewer resources
	- Pre-calculate and cache data
	- Most apps have more reads than writes, perfect for caching
- Save money  
![[Pasted image 20230315171153.png]]
#### 3. Caching Layers
![[Pasted image 20230315172151.png]]
##### 3.1. DNS
- Go to DNS once to get the IP and store it on the client
##### 3.2. CDN
- Content Distribution Network, eg. Cloudflare 
- Store static files like pictures and videos
##### 3.3. Application
##### 3.4. Database
#### 4. Distributed Cache
- Has built-in functionality to replicate data , shared data across servers, and locate proper server for each key
- Replication
- ![[Pasted image 20230315172830.png]]
#### 5. Cache Eviction
##### 5.1. Why?
- Prevent stale data
- Caching only tmost valuable data to save resources
##### 5.2. How
- TTL-Time to live
	- Set a time period before a cache entry is deleted
	- To prevent stale data
- LRU- Least recently used
	- Once cache is full, remove last accessed key and add new key
- LFU-Least frequently used
	- Track number of times key is accessed 
	- Drop least used when cache is full
#### 6. Caching Strategies
#### 7. Cache Consistency
## [[Database]] Scaling and Design 
Performance bottleneck  
Read heavy, around 95%+
### Basic Scaling Techniques
#### 1. Indexes
- Index based on column
- Speeds up read performanceWrites and updates become slightly slower
- More storage required
#### 2. Denormalization
- Go against a standard best practice with relational databases
- Add redundant data to tales to reduce joins
- Boosts read performance
- Slows dorn writes
- Risk inconsistent data across tables 
- Code is harder to write
#### 3. Connection Pooling
- Allow multiple application threads to use same DB connectionSaves on overhead of independent DB connections
#### 4. Caching
- Cache sits in front of DB to handle serving content
- Can't cache everything (Dynamic data)
##### 4.1. Tools
- Redis
- Memcached
#### 5. Vertical Scaling
- Get a bigger server, with fast processor or more memory
### Replication and Partitioning
#### 1. Read Replicas
- Create replica servers to handle reads
- Master server dedicated only to writes
- Have to handle making sure new data reaches replica
#### 2. Sharding
- Horizontal partitioning
#### 3. Vertical Partition
- Divide schema of DB into separate tables
- Generally divide by functionality
- Best when most data in row isn't need for most queries
### When to consider NoSQL
Know what you're gonna sacrifice
- Consistency > SQL
- Scale > NoSQL
## API Design  
## Design a YouTube Clone
#### 1. Requirements
#### 2. Capacity Estimates/ Resources Needed
- Storage
	- ![[Pasted image 20230315181041.png]]
- Bandwidth
	- ![[Pasted image 20230315181229.png]]
#### 3. DB Design
![[Pasted image 20230315181340.png]]
#### 4. System Architecture
![[Pasted image 20230315181512.png]]
#### 5. Specific Components