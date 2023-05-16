---
Title: README-Template
tags: TechSkills
DateStarted: 2023-03-21
DateModified: 2023-03-21
status:
Progress: NaN%
---

## 项目介绍 Project Brief

This is an e-commerce website using MongoDB, Next.js and TailwindCSS, following along [MongoDB Jumpstart Series](https://github.com/mongodb-developer/jumpstart-series) for learning the following skills.

- Use MongoDB with MongoDB Atlas
- Run MongoDB locally and connect it to front-end project

## 核心功能 Core Functions

Fix deprecated function problems in the original project:

- Fix error in using async function in `useEffect`
- Replace deprecated attributes in `next/image`
- Fix infinite loop and routing error in implementing search and autocomplete functions with `next/router`

## 效果展示 Demo

![MongoDB-e-commerce-site](https://images.zsxq.com/FhmLgdNjmMABdO7EATqf25c2ko2G?imageMogr2/auto-orient/thumbnail/800x/format/jpg/blur/1x0/quality/75&e=1682870399&s=vvjvjyvtytyvmy&token=kIxbL07-8jAj8w1n4s9zv64FuZZNEATmlU_Vm6zD:v8Z8NhY92HM7yhzquruuTjAqt68=)

## 使用说明 How to use

### e-commerce-atlas

1. Sign up and create a database in MongoDB Atlas  
      [Log in | MongoDB](https://cloud.mongodb.com/v2/6417bb52bfb15d1d8f3fe4e3#/clusters)
2. run `npm i`
3. create `env.local` file in the project root folder and fill in your database app id `NEXT_PUBLIC_REALM_APP_ID=<Your Realm App ID>`
4. Download sample data from [GitHub - mongodb-developer/jumpstart-series at compass](https://github.com/mongodb-developer/jumpstart-series/tree/compass) and import to your cluster database
5. run `npm run dev` to start developing the project with your remote MongoDB database

## 待办 TODO

### e-commerce-local

- [x] Connect Frontend App with local MongoDB Database

## 参考资料 Reference

[MongoDB Jumpstart Series](https://github.com/mongodb-developer/jumpstart-series)  
[MongoDB: The Developer Data Platform | MongoDB](https://www.mongodb.com/)
