---
title: -tech-stack
type: D
project: Learn-react
category: TechProjects
tags:
  - React
DateDone: 
DateReviewed: 
reviewed: 
difficulty: 
status: 
comment: 
draft: true
DateStarted: 2024-09-19
DateModified: 2024-09-21
mindmap-plugin: basic
---


<%-*  
let  newtitle  
if(tp.file.title.includes("未命名") || tp.file.title.toLowerCase().includes("untitled"))  
{ title=await tp.system.prompt("请输入要创建的文件名");  
  newtitle=title||tp.date.now("YYYYMMDDHHmmss")  
	await tp.file.rename(newtitle)}  
	else newtitle=tp.file.title  
-%>
# <% newtitle %> 

## Version Management

### branch
- main (published)

## Build

### Actions

## Deploy

### Actions

## Commit Convention

### commitizen

## Lint

### antfu-eslint-config
- auto correct syntax error

### headwind
- auto sort tailwind class

## Routing

### Actions

## Style

### Tailwind / UnoCSS

### Icons

## Data-fetching










