---
title: 怎样实现 Obsidian 笔记 Windows 与 iPhone, iPad 同步与备份
tags: PKM/Setup
started: 2023-04-25 Tue
due: 
modified: 2023-04-25 Tue
status: 🟡Organizing
---
## 怎样实现 Obsidian 笔记 Windows 与 iPhone, iPad 同步与备份？
### 注意：慎用 Windows iCloud 同步🚫
1. Windows iCloud 同步一直挂起（pending）无法同步至iOS 移动端，且无法查看同步进度与挂起原因
2. 尝试解决Windows iCloud 同步一直挂起（pending） 的问题，退出iCloud 登录后，再次登录，之前配置信息全无，PC iCloud内资料以及iCloud所在盘其他资料==全被删除== ，未被回收
3. 内容丢失后，PC端丢失内容难以从iCloud恢复
	- iCloud 网页端无法找到PC端显示挂起中后被丢失的文件
	- 其他iOS移动端已同步内容只能单个文件逐一下载至PC，无法整体下载恢复
## 所需服务与费用 💰
#### 1. iCloud
- 8元/月，50G
- 可同步并备份iOS平台内容
#### 2. One Drive
- 15元/月，100G
- 可同步 Obsidian 笔记
- 可备份
- 可查看并恢复单个文件同步历史，PC兼容良好，可配合iCloud实现三端同步
#### 3. 百度网盘
- 25元/月，1000+G
- 可备份，功能齐全
- 易分享，易下载其他百度网盘资源
#### 4. GitHub + Obsidian Git
- 可备份，可进行版本管理
- ! 不宜备份大文件
#### 5. Remotely Save
- 免费，Obsidian 同步插件
- ! 无法同步识别删除内容，无法有效同步插件样式等配置文件

### 具体操作方案 🚀
一定注意定期备份，同步不等于备份！！
#### 1. Obsidian Git
- 备份笔记（除笔记关联图片音视频等大文件）至 GitHub
- 版本历史：可进行版本管理与恢复
#### 2. One Drive 
- 备份笔记文件夹（含笔记关联图片音视频等大文件）
- 版本历史：可对单个文件进行历史版本恢复
	- 选中对应文件，右键单击，选择查看历史
- PC 本地删除
	- ✅网页云端还在，网页云端删除，**网页云端回收站**可恢复
- iOS 本地删除 > 未/已同步至云盘 > 
	- ✅未同步的备份笔记库还在 > 可PC端打开备份笔记库后，重新同步至云 > iOS 打开笔记库重新同步恢复  
	- 也可 iCloud 回收站恢复？ 
#### 3. Remotely Save
- 可 OneDrive, Dropbox, Google Drive 同步
- 将在App文件夹生成同步笔记文件夹，该文件夹为PC, 移动端共享共改的**云端同步笔记**，内容同步由 Remotely Save 控制
	- iOS 本地笔记文件夹由 iCloud 存储管理，通过 Remotely Save 同步 Drive 云端同步笔记内容

![[2023-04-15 2023-04-15 22.08.33.excalidraw]]