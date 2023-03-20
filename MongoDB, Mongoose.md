---
title: MongoDB, Mongoose
tags: Database   
started: 2023-01-09 Mon
due: 
modified: 2023-03-06 Mon
status: 
---
## Reference
[The Principles of Data Modeling for MongoDB - YouTube](https://www.youtube.com/watch?v=YsaOcUDUJKY&t=1085s)
[MongoDB Course Catalog Homepage | MongoDB University](https://learn.mongodb.com/catalog?labels=%5B%22Language%22%5D&values=%5B%22Node.js%22%5D)

## How-to use?
#### 1. Set up a project and create a database in MongoDB Atlas
- Sign up/ in: [Log in | MongoDB](https://cloud.mongodb.com/v2/6417bb52bfb15d1d8f3fe4e3#/clusters)
- Create a project
	- Name your project
	- Add member (Owner is added by default)
- Build a database
	- Add current IP Address
	- Choose a plan (M0-Free)
		- ![[Pasted image 20230320101118.png]]
	- Provider (Azure)
	- Recommended Region (Hongkong)
	- Name for the cluster
		- ![[Pasted image 20230320101328.png]]
- Security > Quickstart
	- Authenticate your connection > Username and password
- Deployment > Database> Load Sample Dataset
	- 8 Databases, 21 collections
#### 2. Connect to MongoDB (with MongoDB Shell/ application/ Compass/ VS Code)
- Connect > Copy connection string
- Install [[VS Code]] Extension > MongoDB for VS Code
##### 2.1. MongoDB Compass
- Use cases
	- Visually explore data
	- Run **ad hoc queries**
	- Full CRUD functionality
	- Query performance
	- Construct **aggregation**s...
- Create Database > Collection
- Import sample data
	- [GitHub - mongodb-developer/jumpstart-series at compass](https://github.com/mongodb-developer/jumpstart-series/tree/compass)
#### 3. MongoDB Realm - Serverless Platform/ Backend as a service (without having to set up your own ==server==)
- Install Realm SDK:
	- [Install Realm - Web SDK — Realm](https://www.mongodb.com/docs/realm/web/install/#std-label-web-install)
- Connect Realm with a Next.js web app
	- [Next.js Integration Guide - Web SDK — Realm](https://www.mongodb.com/docs/realm/web/nextjs/)
	- [How to connect your NextJs app to MongoDB - YouTube](https://www.youtube.com/watch?v=mOvW3iheF14)
- Use Cases
	- Easily and securely access data from MongoDB Atlas database and bring our data into our applications
	- Functions
	- User authentication
	- Triggers
		- User authentication events
		- Preset schedule
	- Data access control
	- 3rd party services
	- GraphQL...
	- Realm sync (Sync data among different devices in real time)
#### 4. Frontend MongoDB Integration
- `npm i @heroicons/react`
#### 5. Search and autocomplete with MongoDB Atlas
- Lucene powered search engine
- Typo tolerance with fuzzy search
- Autocomplete
- Filters & Facets
- Custom sorting...

## Teminology difference
![[Pasted image 20230320083604.png]]
## Query Language > MQL

## Options
#### 1. Self-hosted
- Open source MongoDB server
#### 2. MongoDB Atlas
- SAAS
#### 3. MongoDB Compass
- GUI
#### 4. MongoDB Realm
#### 5. MongoDB Atlas Search
#### 6. MongoDB Charts
#### 7. MongoDB Online Archive
#### 8. MongoDB Atlas Data Lake
## Challenges
![[Pasted image 20230320070956.png]]
### Data Model
#### 1. Challenges
- Collections
- Structure of documents
- How relationships are modeled
- Too denormalized
#### 2. Determines Performance
- How to deal with `join`?
![[Pasted image 20230320071530.png]]
## Schema and Data Modeling
### The need to model for NoSQL
To face and answer to Constrains (physical, hardwre, software)
![[Pasted image 20230320072127.png]]
#### 1. SQL Approach (3rd normal form)
![[Pasted image 20230320072225.png]]
#### 2. MongoDB Approach
![[Pasted image 20230320072315.png]]

### Techniques to model for MongoDB
#### 1. Methodology
![[Pasted image 20230320072445.png]]
#### 2. Different thinking procedures
![[Pasted image 20230320072640.png]]
#### 3. Analyze the workload
- Listing operations
	- ![[Pasted image 20230320072739.png]]
- Details for an operation
	- ![[Pasted image 20230320072903.png]]
#### 4. Identify relationships
- Different Data Modeling
	- ![[Pasted image 20230320073319.png]]
- Criteria: What is used together in the application is stored together in the database.
##### 4.1. Two ways of modeling relationships
![[Pasted image 20230320073743.png]]
- Reference/Link
	- when the "many" side is a huge number
	- for integrity on write operations on many-to-many
	- when a piece is frequentyly used but not the other and memory is an issue
- Embeding (using one collection)
	- for integrity of read operations
	- for integrity of write operations on one-to-one and one-to-many
	- for data that is deleted or archived together
	- by default
##### 4.2. Design Patterns
![[Pasted image 20230320080304.png]]
### Evolving the model with the "Schema versioning" pattern
Applying the **extended reference, computed, subset, schema versioning** patterns:
![[Pasted image 20230320080750.png]]
schema versioning pattern is to optimize the releasing process
![[Pasted image 20230320081256.png]]