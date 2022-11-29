---
title: Obsidian-使用指南
tags: 工具方法/Obsidian
status: Doing
started: 2022-11-21
closed: 2022-11-25
aliases: 
---
## 通用
##### 1. 快速搜索相关内容？`CTRL + F` / `CTRL + SHIFT + F`
##### 2. [[Obsidian-插件功能#Quick Switcher++|快速查找并打开]] 对应文件/视图？`Alt + F` / `CTRL + O`
##### 3. 快速调用相关功能？`ctrl + P`
## 视图
##### 1. 快速 [[Obsidian-插件功能#Quick Switcher++|切换视图]]？
- `Alt + F` > `edt + space + 视图名称`
##### 2. 快速打开对应 [[Obsidian-插件功能#⬇️视图插件|视图]]？
- Graph: `CTRL + SHIFT + G` / `Ctrl + G`
- Backlink: `CTRL + SHIFT + B` 
- Outgoing-link: `CTRL + SHIFT + O` 
- Outline: `Shift + O` 
- Timeline: `Ctrl + Shift + P`
- Calendar: `Ctrl + Shift + C`
- Tags: `CTRL + SHIFT + A`
- Split to right: `CTRL + ALT + S`
- File Explorer: `ALT + L` 
##### 3. 任意调整 [[Obsidian-插件功能#Custom File Explorer Sorting|文件夹顺序]]？
##### 4. 笔记中自动生成并插入笔记内容大纲（[[Obsidian-插件功能#Dynamic Table of Content|Table of Content]]）？
## 编辑
##### 1. Heading: `ctrl + 1/2/...`
##### 2. Link：`ctrl + shift + L`
##### 3. List：`ctrl + alt + L`
##### 4. Checkbox: `ctrl + L`
##### 5. Move line up/ down: `alt + up/ down`
##### 6. [[Obsidian-插件功能#Highlightr|Hightlight]]: `ctrl + alt + H/ B/ R/ Y/ G`; `alt + H`
##### 7. Date: 快速插入日期、时间？`CTRL + ALT + D` / `ALT + T`
##### 8. Delete: 快速删除整行？`CTRL + D`
##### 9. [[Obsidian-插件功能#Admonition|Callouts]]: `CTRL + ALT + O`
##### 10. 全局查找替换，删除所有空行 (blank line)?
- [[快捷键#VS Code Keyboard Shortcuts|VS Code]]：🟩
	- [[快捷键#VS Code Keyboard Shortcuts|快捷键]]：打开“查找与替换” `ctrl + shift + F`
	- 查找 > 输入 `^$\n`
	- 替换 > 不输入任何内容
	- 确认：`ctrl + alt + enter`
	- 参考链接：[vim-delete-line](https://linuxize.com/post/vim-delete-line/)
- Vim 模式：🟨
	- 打开 editor > vim-key-binding
	- 打开对应文档，输入 `:%s/^$\n*//g`
	- 参考链接：[Remove All Blank Lines In File - Resolved help - Obsidian Forum](https://forum.obsidian.md/t/remove-all-blank-lines-in-file/35082)
## 样式
##### 1. 快速调整[[工具推荐：一款好用且免费的笔记软件 Obsidian-2|图片样式、尺寸]]？🟩
##### 2. [[Obsidian-插件功能#Linter|自动纠正]] 文本样式（列表序号，Yaml 时间）？`ALT + L`
##### 3. 自动 [[Obsidian-插件功能#MetaEdit|设置Yaml]] 内容？
##### 4. 自动为文档 [[Obsidian-插件功能#Number Heading|标题编号]]？
##### 5. 调整代码块样式，显示 [[Obsidian-插件功能#Better CodeBlock|代码标题]] 和行数？
##### 6. [[Obsidian-插件功能#⬇️样式插件|自定义样式]]（字号、标题、行间距）？
##### 7. 自动生成 [[Obsidian-插件功能#Auto Link Title|链接标题]]？
## 任务追踪
##### 1. 高效[[Obsidian-插件功能#Day Planner|追踪学习进展]]与阶段成果？
## 表格
##### 1. 自定义 [[Obsidian-插件功能#Tableview|生成表格]]？
##### 2. 快速 [[Obsidian-插件功能#Advanced Table|创建表格]]？
## 模板
##### 1. 快速插入模板？`CTRL + ALT + T`
##### 2. 快速调用 [[Obsidian-插件功能#Templater|代码模板]] 自动化批量处理？
## 备份
##### 1. [[Obsidian-插件功能#Imgur Plugin|自动上传图片]]，生成图片链接？

## 学习记录

```dataview
TABLE title, started, status
WHERE contains(title, "Obsidian")
SORT started DESC
```