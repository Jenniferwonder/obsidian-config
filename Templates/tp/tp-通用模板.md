---
<%-* 
let  newtitle
if(tp.file.title.includes("未命名") || tp.file.title.toLowerCase().includes("untitled")) 
{ title=await tp.system.prompt("请输入要创建的文件名");
  newtitle=title||tp.date.now("YYYYMMDDHHmmss")
	await tp.file.rename(newtitle)}
	else newtitle=tp.file.title
-%>

UID: <% tp.date.now("YYYYMMDDHHmmss") %> 
title: <% tp.file.title %> 
tags: 
started: <% tp.date.now("YYYY-MM-DD") %>
modified: <%+ tp.file.last_modified_date("YYYY-MM-DD dddd HH:mm:ss") %>
status: <% tp.system.suggester(["⚪Capturing", "🟡Organizing", "🟠Distilling","🟢Published","🔵Archived"], ["⚪Capturing", "🟡Organizing", "🟠Distilling", "🟢Published", "🔵Archived"]) %>
due:
cssclass: 
---
## Purpose

## Problems

## Solutions


## Highlights


## Reflections

## Related Notes

## Reference


