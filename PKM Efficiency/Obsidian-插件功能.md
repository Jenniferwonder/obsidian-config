---
title: Obsidian-插件功能
started: 2022-11-24 Thu
modified: 2023-04-18 Tue
status: 🟠Distilling
due: 
---
## 💡Improvement Ideas
从链接或图片，截图取文字

## ⬇️备份与同步
[[Sync and Back up]]
#### 1. Obsidian Git
- 备份笔记（除笔记关联图片音视频等大文件）至 GitHub
#### 2. One Drive 
- 备份笔记文件夹（含笔记关联图片音视频等大文件）
- PC 本地删除
	- ✅网页云端还在，网页云端删除，**网页云端回收站**可恢复
- iOS 本地删除 > 未/已同步至云盘 > 
	- ✅未同步的备份笔记文件夹还在 > 可PC端打开后，重新同步至云 > iOS 打开重新同步恢复  
	- 也可 iCloud 回收站恢复？ 
#### 3. Remotely Save
- 可 OneDrive, Dropbox, Google Drive 同步
## ⬇️思维导图与白板
#### 1. Excalidraw
- [[Excalidraw]]
#### 2. Markmind
- [[Mindmap]]
#### 3. Canvas
- [[Canvas in Obsidian]]
- Link Exploder
- Link Note in Canvas
- Canvas Mindmap
- Canvas Presentation
- Optimize Canvas Connections 
## ⬇️效率进阶
### 模板工具
#### 1. QuickAdd
- [[QuickAdd in Obsidian]]
#### 2. Templater
- 使用代码模板自动化批量处理任务
- [[Templater in Obsidian]]
#### 3. Buttons
- 支持添加自定义功能按钮
#### 4. Advanced URI
#### 5. Virtual Hotkey Keyboard 
- 展示快捷键键盘
#### 6. Auto Note Mover
- 可根据标签或标题，自动移动笔记到对应文件夹
#### 7. Remember Cursor Position
- 记住每篇笔记光标所在位置，并自动定位
#### 8. AI 工具🟡
- [[AI Tools]] 

## ⬇️项目管理视图进阶
#### 1. Homepage
#### 2. Workspaces-plus (+Workspace)
#### 3. DB Folder
#### 4. Projects
#### 5. Longform
#### 6. Tableview
- 自定义条件生成表格视图
- 时间格式：file.cday/ file.ctime; file.mday/ file.mtime
## ⬇️知识切割与复习 Distill
#### 1. Note Refactor
- 按指定条件分割笔记成新笔记
#### 2. Spaced Repetition
![[Pasted image 20230419095220.png]]
#### 3. Flashcard
- [[Anki Flashcard Review]]
## ⬇️学习记录 Capture > Organize
### 网页浏览与搜索
#### 1. Omnisearch
- 可搜索网页并收藏
#### 2. Surfing
- 可在 Obsidian 浏览网页
### 阅读批注
#### 1. Annotator
- PDF 资料文件夹 > Annotator > PDF 阅读批注
#### 2. Weread Plugin
- 同步微信读书
### 图片批注
#### 1. 方案一：One Drive + Remotely Save + PDF in Obsidian
- 打开 One drive 网盘 > 笔记拍照 > 批注 > 生成PDF文件 > 存回笔记文件夹 > Remotely Save 同步 

### 视频笔记

### 音频笔记
#### 1. Podnotes
- 自动为音频添加 Timestamp，并支持跳转
- `Ctrl`+`Alt`+`P` 添加时间戳链接

## ⬇️展示
#### 1. Advanced Slide
- Markdown 转 PPT

## ⬇️导出与分享
### 图片上传
#### 1. Imgur Plugin
- 可自动上传图片至 Imgur🟡
### 笔记导出
#### 1. Pandoc Plugin
- 支持多种格式导出笔记
### 网页发布分享
#### 1. Webpage HTML Export
- 将笔记导出为HTML网页格式，含黑白模式切换

## ⬇️编辑输入与快速查找
### 快速查找
#### 1. Quick Switcher++
- 启动查找/ 切换视图/ 打开对应文件：`ALT + F`
### 快速编辑
#### 1. Linter
- 可自动纠正文本样式（列表序号）
#### 2. ~~MetaEdit~~ (> Metadata Menu)
- `ALT`+`M`
- 可自动设置 Yaml 格式
- 配合 Linter，更新 Yaml 内容
#### 3. Metadata Menu（配合DB Folder/ Projects）
- 配置管理Metadata
- 自动提供可选填充项
#### 4. Number Heading
- 可自动为标题编号，可自定义编号样式
#### 5. Auto Link Title
- 可自动生成链接标题
#### 6. Multi-Column Markdown
- 可支持同一笔记多栏布局（文案 + 分镜概要）
#### 7. Hover Editor
- 支持编辑预览弹框
#### 8. Citation/ Footnote
- 快速添加脚注
### 快速输入
#### 1. Various Complements
- 可提示相关文本，快速填充
#### 2. ~~讯飞输入法~~
- 自定义快捷输入、语音输入、多端同步
### 其他可选编辑（Optional）
#### 1. Table Enhancer
- 鼠标右键直接创建指定规格表格，并可右键单击对应区域调整编辑
#### 2. Markdown Table Editor
- 提供Markdown表格编辑器
- 可打开其他格式表格
#### 3. Advanced Table
- 快速创建表格
#### 4. Natural Language Dates
- 可自动生成日期
#### 5. Supercharged Links
- 可自定义链接样式
#### 6. Admonition
- 可美化、快速插入 Callout
#### 7. cMenu/ MAKE
- UI 编辑器
## ⬇️样式美化
### 通用样式美化
#### 1. Minimal/ Blue Topaz
- 可快速设置主题样式
#### 2. Minimal Theme Settings
- 可调整 Minimal 主题样式
#### 3. Style Settings
- 可自定义样式
#### 4. Contextual Typography
- 可自定义文本样式
### 其他样式美化
#### 1. Better Word Count
- 可显示笔记字数或选中片段字数
#### 2. Better CodeBlock
- 可在阅读视图，显示代码标题
#### 3. Highlightr
- 可自定义、快速高亮
#### 4. Hide Sidebars on Window Resize
- 可在窗口缩小时隐藏边栏
#### 5. Folder Icon
- 为文件夹添加Icon
## ⬇️核心视图功能
### 日历
#### 1. Calendar
- 可形成日历视图
- 可创建并追踪每日日记
### 大纲
#### 1. Dynamic Table of Content/ Floating-toc
- 可在笔记中自动生成并插入笔记内容大纲
#### 2. Outliner
- 可形成大纲视图 
- 可强化列表快捷键功能
#### 3. Quite Outline
- 可选择展开相应层级标题
![[Pasted image 20230419095832.png]]
### 标签
#### 1. Tag Wrangler
- 可修改全局标签
### 文件夹
#### 1. Custom File Explorer Sorting/ MAKE
- 可自定义文件夹排序优先级
#### 2. File Tree Alternative Plugin
- 可打开子文件夹视图
#### 3. Quick Explorer
- 可查看笔记所在文件夹路径
#### 4. Recent Files
- 可显示最近打开文件列表
#### 5. Folder Note
- 支持点击文件夹后，显示文件夹同名笔记
#### 6. Waypoint
- 自动在文件夹同名笔记生成文件夹所含笔记链接
### 任务追踪视图
#### 1. Checklist
- 提高任务清单效率  
#### 2. Task
- 定义检索任务状态，自动添加完成任务时间
#### 3. Heatmap Calendar
- 追踪目标、习惯、任务、运动、财务等
## ⬇️周期记录
#### 1. Daily Note (Core Plugin)
- 可自动创建每日日记
#### 2. Day Planner
- 可形成 Timeline 视图
- 可自动检测时间，更新任务状态，提高任务追踪效率
#### 3. Periodic Notes
- 创建对应周记、月记、年记