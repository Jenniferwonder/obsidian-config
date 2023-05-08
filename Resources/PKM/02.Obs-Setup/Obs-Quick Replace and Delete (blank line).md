---
Title: Obs-Quick Replace and Delete (blank line)
tags:
DateStarted: 2023-04-21
due:
DateModified: 2023-04-21
status:
---

## 全局查找替换，删除所有空行 (blank line)?

#### 1. 方案一：VS Code

- [[Keyboard-Shortcuts#VS Code Keyboard Shortcuts|VS Code]]：🟩
  - [[Keyboard-Shortcuts#VS Code Keyboard Shortcuts|快捷键]]：打开“查找与替换” `ctrl + shift + F`
  - 查找 > 输入 `^$\n`
  - 替换 > 不输入任何内容
  - 确认：`ctrl + alt + enter`
  - 参考链接：[vim-delete-line](https://linuxize.com/post/vim-delete-line/)

#### 2. 方案二：Vim 模式

- Vim 模式：🟨
  - 打开 editor > vim-key-binding
  - 打开对应文档，输入 `:%s/^$\n*//g`
  - 参考链接：[Remove All Blank Lines In File - Resolved help - Obsidian Forum](https://forum.obsidian.md/t/remove-all-blank-lines-in-file/35082)
