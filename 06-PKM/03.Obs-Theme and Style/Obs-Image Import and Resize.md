---
title: 图片插入与尺寸调节方法
tags:   
started: 2023-04-21 Fri
due: 
modified: 2023-04-21 Fri
status: 🟠Distilling
---
Orginal: [[Obsidian Post-2]] 
# Obs-图片插入与尺寸调节方法
#### 1. Markdown 本地图片链接

```markdown
![[Pasted image 20221124194000.png| 400]] //Obsidian ![[本地文件路径 | 尺寸参数]]
![Pasted image 20221124194000](E:...\assets\Pasted image 20221124194000.png) //Typora
```

#### 2. Markdown 网络图片链接

```markdown
![|400](https://cdn.nlark.com/yuque/0/2022/png/29677165/1669290486575-4a3d3b02-8311-4a0f-a0be-273db6779bd2.png) //Obsidian & Typora
```

#### 3. HTML 标签

```markdown
<img src="https://cdn.nlark.com/yuque/0/2022/png/29677165/1669290486575-4a3d3b02-8311-4a0f-a0be-273db6779bd2.png" style="height: 60%" /> //Obsidian
<img src="https://cdn.nlark.com/yuque/0/2022/png/29677165/1669290486575-4a3d3b02-8311-4a0f-a0be-273db6779bd2.png" style="zoom: 60%" /> //Typora
```

### 如何替换Typora不兼容的图片尺寸参数？
可用 VS Code 打开笔记文件夹，`CTRL + SHIFT + F` 一键查找全局替换，比如：Typora HTML 图片标签中的 `zoom` 可替换为 `height` / `width` 。  
Typora `style="zoom:50%"` 约相当于 Obs `style="height:50%"` 。  
### 效果展示
- ![|400](https://cdn.nlark.com/yuque/0/2022/gif/29677165/1669345223674-b01bf6c6-aa61-433d-9ae4-d2c0e6df9a3e.gif)