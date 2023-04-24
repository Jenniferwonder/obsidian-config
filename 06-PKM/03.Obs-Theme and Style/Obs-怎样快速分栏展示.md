---
title: Obs-怎样快速分栏展示
tags:   
started: 2023-04-21 Fri
due: 
modified: 2023-04-23 Sun
status: 
---
## 需求
类似上一篇、前一篇分两栏展示功能
## 方案二：Multi-Column Markdown 插件 (手机兼容？)

## 方案一：通过Blue Topaz 内置自定义 Admonition 样式
### 实现猜想
通过Blue Topaz 内置自定义 Admonition 样式
### 资料参考
[[分栏效果示例]]
### 实践

````ad-col2
title: 相关笔记
color: 99,178,129
collapse: open
```ad-blank
**Previous**

```
```ad-blank
**Next**

```
````

### 成果
创建两栏模板：[[Ad-two-column-simple]]