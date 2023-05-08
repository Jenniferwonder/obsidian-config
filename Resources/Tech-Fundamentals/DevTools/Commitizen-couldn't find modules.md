---
Title: "couldn't find modules"
tags: [Tech-Fundamentals]
DateStarted: 2023-04-24 Mon
DateModified: 2023-04-24 Mon
due:
uid: 20230424142352
cssclass:
status:
---

[[前端大全]]

## Problems/Purpose

Windows 下载 Commitizen 改善 Github 代码/笔记提交规范
全局下载至 C 盘，F 盘出现报错“Couldn't Find Modules”

## Solutions

`--force`

## Highlights

`npm i -g commitizen`
`npm i -g cz-conventional-changelog`
如果是 Ubuntu, `echo '{"path":"cz-conventional-changelog"}' > ~/.czrc`
`commitizen init cz-conventional-changelog --save --save-exact`

- 如果报错，上一行命令后加`--force`

### 运行使用

- `git add`
- `git cz`

## Reflections

## Reference
