---
<%-* 
let  newtitle
if(tp.file.title.includes("未命名") || tp.file.title.toLowerCase().includes("untitled")) 
{ title=await tp.system.prompt("请输入要创建的文件名");
  newtitle=title||tp.date.now("YYYYMMDDHHmmss")
	await tp.file.rename(newtitle)}
	else newtitle=tp.file.title
-%>
<%-*
var cleanTitle = tp.user.getTitleSnippet(newtitle) 
var title = `${cleanTitle}`;
await tp.file.rename(`${title}`);
let filetype = await tp.system.suggester(["Projects", "Tech-Fundamentals", "Front-End", "PKM"], ["Projects", "Tech-Fundamentals", "Front-End", "PKM"], false, "路径放到哪里？") 
if (filetype === "Projects") { 
myFilePath = "/03-Projects/00-Inbox/" +  `${title}`;
await tp.file.move(`${myFilePath}`);
} else if (filetype === "Tech-Fundamentals") { 
myFilePath = "/04-Tech-Fundamentals/00-Inbox/" +  `${title}`;
await tp.file.move(`${myFilePath}`);
} else if (filetype === "Front-End") { 
myFilePath = "/05-Front-End Tech Stack/00-Inbox/" +  `${title}`;
await tp.file.move(`${myFilePath}`);
} else if (filetype === "PKM") { 
myFilePath = "/06-PKM/00-Inbox" +  `${title}`;
await tp.file.move(`${myFilePath}`);
} else { 
myFilePath = "01-Inbox" +  `${title}`;
await tp.file.move(`${myFilePath}`);
}
-%>
title: <% `${title}` %> 
tags: <% `${filetype}` %>
started: <% tp.file.creation_date() %>
uid: <% tp.date.now("YYYYMMDDHHmmss") %> 
cssclass: 
---

## Metadata
Status::    <% tp.system.suggester(["⚪Captured", "🟡Organized", "🟠Distilled","🟢Published","🔵Archived"], ["#Status/⚪Captured", "#Status/🟡Organized", "#Status/🟠Distilled", "#Status/🟢Published", "#Status/🔵Archived"]) %>
Topic:: [[<% tp.system.prompt("这个笔记对应的主题MOC ", "比如：时间管理") %>]]
Source Type::  <% tp.system.suggester(["💭想法", "📚书籍", "📰️文章", "🗣️聊天", "💻教学", "▶️视频", "🎧️播客"], ["#📥/💭想法 ", "#📥/📚书籍 ", "#📥/📰️文章", "#📥/🗣️聊天 ", " #📥/💻教学", "#📥/▶️视频", "#📥/🎧️播客"]) %>
Author:: 
Source URL:: 

## Problems/Purpose
Summary:: 
## Solutions


## Highlights


## Reflections

## Reference
