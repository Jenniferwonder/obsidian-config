---
title: JS 方案要点：CSS, HTML，原生 JS, jQuery...
tags: 
status: 
started: 
due: 
aliases: 
---
创作时间：2022 年 11 月 7 日
前端学习：第 164 天 
创作打卡：第 13 天
## 文件架构

```markdown
┣ public
 ┃ ┣ css
 ┃ ┃ ┣ blog.css
 ┃ ┃ ┣ editor.css
 ┃ ┃ ┗ home.css
 ┃ ┣ img
 ┃ ┣ js
 ┃ ┃ ┣ blog.js
 ┃ ┃ ┣ editor.js
 ┃ ┃ ┣ firebase.js
 ┃ ┃ ┗ home.js
 ┃ ┣ blog.html
 ┃ ┣ editor.html
 ┃ ┗ home.html
 ┣ .gitignore
 ┣ package-lock.json
 ┣ package.json
 ┣ README.md
 ┗ server.js
```

## HTML 的核心骨架
- 开发环境：VS Code
- `!`+`enter`：emmet 一键生成 HTML 主要标签骨架
   - 效果图：![image.png](https://cdn.nlark.com/yuque/0/2022/png/29677165/1667799092602-a2e20f75-5d68-4cab-a76b-8857e9937489.png#averageHue=%23282a37&clientId=ubda5d380-5cca-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=122&id=uf5b3872c&margin=%5Bobject%20Object%5D&name=image.png&originHeight=243&originWidth=680&originalType=binary&ratio=1&rotation=0&showTitle=false&size=20125&status=done&style=none&taskId=u28f12d2b-8a84-47a9-a9de-c40573411ad&title=&width=340)
### 核心骨架——<head>标签中有哪些标签，作用是什么？
#### SEO 优化
- **<title></title> **添加网站** 标题**
- **<meta>** 添加网站 **描述**
   - name = "description" 
   - content="<描述内容>"
- **<meta>** 使用 “[Open Graph Meta Tags](https://ahrefs.com/blog/open-graph-meta-tags/)”：优化链接分享呈现效果
   - property="**og:**description/ og: title/ og:type/og:url/ og:image/ og:determiner/ og:locale"
   - content="<相应属性内容>"
#### 链接<link>：链接样式表/ 外部样式库
- **<link>**
   - href="<路径>"
   - rel="stylesheet"

```html
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<meta name="theme-color" content="#99D6EA" />
<!-- 添加描述-->
<meta
  name="description"
  content="App created to improve Japanese language skills by daily writing down the users thoughts in the online journal."
/>
<!-- 添加标题-->
<title>Nikki - My Diary Learning App</title>
<!-- 运用 Open-Graph 优化链接呈现效果-->
<meta
  property="og:description"
  content="App created to improve Japanese language skills by daily writing down the users thoughts in the online journal."
/>
<meta property="og:title" content="Nikki - My Diary" />
<meta property="og:type" content="website" />
<meta property="og:url" content="https://nikki-my-diary.netlify.app/" />
<meta
  property="og:image"
  content="https://github.com/YuriDevAT/nikki-my-diary/blob/main/public/thumbnail-nikki.png"
/>
<meta property="og:determiner" content="" />
<meta property="og:locale" content="en_US" />
<!-- 链接外部样式库/ 本地样式表 -->
<link rel="manifest" href="%PUBLIC_URL%/manifest.json" />
<link
  rel="stylesheet"
  href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css"
/>
```

#### 加载优化
- 脚本标签 <script>：链接 JS 文件/ 页面交互效果库
   - src="<路径>"
### 核心骨架——<body>中的标签与结构
#### 链接<a>：路由问题
- 无框架如何搭建多页面网站，实现链接页面跳转？
#### 
