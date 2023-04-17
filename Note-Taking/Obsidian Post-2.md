---
modified: 2023-03-07 Tue
title: Obsidian Post-2
tags: Learning-Efficiency/Note
status: 
started: 2022-11-25 Fri
due: 2022-11-25
---
工具推荐：一款好用且免费的笔记软件 Obsidian-2
## 前言
语雀是国内目前纯净好用功能强大的一款笔记软件，但其开始针对个人用户按月收费，免费笔记数量受限，给大家推荐一款国外开源的笔记软件 **Obsidian**，支持 Markdown，多种视图及内容关联，功能强大，几乎可平替语雀，好用无广告、安全纯净且免费，支持大量好用插件，有中文版，社区活跃，感兴趣小伙伴可以下载尝试！（官方下载链接：[Obsidian](https://obsidian.md/)）
## 笔记软件使用体验对比
- **Typora、语雀、Obsidian** 都是纯净优秀的笔记软件
- **Typora**：最佳 Markdown 编辑器，能全键盘流畅操作，缺点：视图与其他功能有限，无法体现笔记关系
- **语雀：** 一流用户界面，操作简单友好，分享便捷，多端同步，最大缺点：要付费，功能主题样式快捷键均无法自定义，键盘操作不够友好（但看重多端同步与分享的小伙伴，推荐首选语雀）
#### 1. 选择 Obsidian 最重要的原因
- 免费、安全、功能强大，基本具备 Typora、语雀所有功能（除入门和配置有技术难度），且没有以上两款软件的缺点
- 能自定义几乎所有快捷键，支持全键盘快速操作
- 革新文件夹管理笔记思想，支持建立笔记间联系，自动生成关系网，能不断深化完善知识体系，同时支持多种视图快速切换：标签、关系网、时间线、链接、任务、大纲等，即使没有文件夹也能迅速查找并打开对应笔记
- 支持打开多份笔记，竖排呈现，同时编辑
- 支持代码模板，可一键替换或批量处理笔记内容
- 支持每日任务追踪，任务视图可管理所有笔记代办事项
- ……
#### 2. 使用 Obsidian 温馨提示
1. 配置和上手还是有些技术难度的，但是上手后简直刷新对笔记的认识
2. 笔记将保存在本地，可创建 GitHub 私人仓库，或用网盘备份
3. 发布分享、协同编辑功能建议考虑其他途径
4. 插入图片默认保存在本地，支持 Picgo/ Imgur 自动上传，不想配置图床的同学可以考虑将图片先粘到语雀，再复制到 Obsidian 笔记，毕竟语雀的羊毛还是可以薅的 😂 
#### 3. Obsidian 界面效果图（可自定义主题）
![](https://cdn.nlark.com/yuque/0/2022/png/29677165/1669290486575-4a3d3b02-8311-4a0f-a0be-273db6779bd2.png)

## Typora 转 Obsidian，图片格式兼容吗？
亲测兼容没问题，Obsidian (v1.0.3) 与 Typora 均支持并兼容三种 Markdown 或 HTML 本地及外链图片插入方法！
### 图片插入与尺寸调节方法
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

### 如何替换不兼容的图片尺寸参数？
可用 VS Code 打开笔记文件夹，`CTRL + SHIFT + F` 一键查找全局替换，比如：Typora HTML 图片标签中的 `zoom` 可替换为 `height` / `width` 。  
Typora `style="zoom:50%"` 约相当于 Obs `style="height:50%"` 。  
### 效果展示
- ![|400](https://cdn.nlark.com/yuque/0/2022/gif/29677165/1669345223674-b01bf6c6-aa61-433d-9ae4-d2c0e6df9a3e.gif)  
注：以上为个人使用体验，仅供大家参考！大家可根据自身情况，选择最适合自己的笔记软件。😄

## 参考链接
1. [Image zoom: click + hold to expand images - Share & showcase - Obsidian Forum](https://forum.obsidian.md/t/image-zoom-click-hold-to-expand-images/5164)
2. [Workflow: Typora & Obsidian - Share & showcase - Obsidian Forum](https://forum.obsidian.md/t/workflow-typora-obsidian/650/12)
## 原文链接
1. 掘金：[工具推荐：一款好用且免费的笔记软件 Obsidian - 掘金](https://juejin.cn/post/7169838406933938212)
2. 知乎：[工具推荐：一款好用且免费的笔记软件 Obsidian - 知乎](https://zhuanlan.zhihu.com/p/586626931)
3. 知识星球 - 编程导航：[有语雀、Typora，笔记软件为什么用Obsidian？- 知识星球-编程导航](https://articles.zsxq.com/id_j880bpo7922w.html)
4. 知识星球 - 前端宝藏：[有语雀、Typora，笔记软件为什么用Obsidian？- 知识星球-前端宝藏](https://articles.zsxq.com/id_lw6x3omws27c.html)

---




