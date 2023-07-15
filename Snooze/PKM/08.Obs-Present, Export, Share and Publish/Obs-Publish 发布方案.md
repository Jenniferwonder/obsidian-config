---
Title: Obs-Publish 发布方案
tags: PKM
DateStarted: 2023-05-10
DateModified: 2023-05-27
Progress: NaN%
---
# Obs-Publish 发布方案
## Metadata
### Relationships
- Topic:: [[PKM]]
- Up:: [[08.Obs-Present, Export, Share and Publish]]
- Related:: [[pandoc如何使用自定义样式导出docx文档_pandoc自定义docx样式_coderFY的博客-CSDN博客]], [[Obs-Image Import and Resize]]
- SourceURL:: [发布方案](https://www.gachi.cn/%E8%BD%AF%E4%BB%B6%E4%BD%BF%E7%94%A8/obsidian/%E5%8F%91%E5%B8%83%E6%96%B9%E6%A1%88/)
## 网页发布分享
#### 1. Webpage HTML Export
- 将笔记导出为 HTML 网页格式，含黑白模式切换
#### 2. 飞书文档发布教程？
- https://kknwfe6755.feishu.cn/docs/doccnBfbtETItLHMmbDBGBRdPrh#g8Cm9V
## Obsidian 的发布方案[^1]
我选择的是最省事的 Digital Garden 插件配合 github 和 vercel 将文章发布到公网。  
这是我的首页供大家参考：[Welcom](https://www.gachi.cn/)  
其他关于发布的拓展与问题解决可以看：[obsidian](https://www.gachi.cn/%E8%BD%AF%E4%BB%B6%E4%BD%BF%E7%94%A8/obsidian/obsidian/)
### 为什么选择 Digital Garden 作为我的发布方案
Digital Garden 插件发布文章十分简单，通杀 Digital Garden 还适配 [Obsidian](https://www.gachi.cn/%E8%BD%AF%E4%BB%B6%E4%BD%BF%E7%94%A8/obsidian/obsidian/) 主题作为网站主题，支持双链、等等许多优点。配合 vercel 的自动构建和 CDN 基本上能烦恼我的就只有文章该怎么写这种世纪难题了。
### 搭建和部署
#### 1. 所用到的工具和网站
- Digital Garden： [GitHub - oleeskild/obsidian-digital-garden](https://github.com/oleeskild/obsidian-digital-garden)
- 插件文档地址： [Digital Garden Overview](https://dg-docs.ole.dev/)
- Vercel：[Vercel: Develop. Preview. Ship. For the best frontend teams](https://vercel.com/)
#### 2. 部署步骤
参考： [01 Getting started](https://dg-docs.ole.dev/getting-started/01-getting-started/)
1. 在 [Obsidian](https://www.gachi.cn/%E8%BD%AF%E4%BB%B6%E4%BD%BF%E7%94%A8/obsidian/obsidian/) 中下载 Digital Garden 插件
2. 根据文档提示在 [GitHub - oleeskild/digitalgarden](https://github.com/oleeskild/digitalgarden) 这个仓库中点击 Deploy 即可自动构建仓库和 Vercel 项目 ![image.png](http://cdn-ob-pic.hningyun.com/simp/202303271454722.png-shoushen)
3. 等待项目构建完成后进入这个 [链接](https://github.com/settings/tokens/new?scopes=repo) 会自动为你创建条件合适的 token，如果不想过几个月就更新一下 token 可以选择将过期时间改为永久，默认是三十天，当然如果当心安全问题，也可以自己为单独的仓库设置 token 但是过期时间无法设置为永久，过程比较简单我就不一步一步去详述了
4. 将刚刚获取到的 token 和你的 github 账号名和仓库名称填入插件中 ![image.png](http://cdn-ob-pic.hningyun.com/simp/202303271501423.png-shoushen)
5. 配置到这就结束了，肥肠的简单
#### 3. 插件的设置
一定要关闭Slugify Note URL这个选项  
根据这篇[issue](https://github.com/oleeskild/obsidian-digital-garden/issues/125)，不关闭这个选项会在项目构建中对文件名进行路径处理，而如果路径中含有非英文字符则会构建失败导致无法访问这篇文章  
下面是我的设置，有需要的同学可以参考  
![image.png](http://cdn-ob-pic.hningyun.com/simp/202303271516314.png-shoushen)

### 如何发布文章

```
dg-publish: true
dg-home: true
```

1. dg-home 是告诉插件这篇文章应该是你的主页。(它只需要添加到一个笔记，而不是你要发布的每个笔记)。
2. dg-publish 设置告诉插件这个注释所在的文章需要发布。没有此设置的注释将无法发布。(换句话说: 你发布的每个笔记都需要这个设置。)
3. 通过在 Windows/Linux（Mac 上的 CMD+P）上按 CTRL+P 打开您的命令板，然后找到“Digital Garden: Publish Single Note”命令。按 Enter。就能发布当前笔记了

### 完成
现在已经完成了网站的构建和发布，是不是非常的简单。最后需要注意的一点 Digital Garden 构建的网站不支持网站内中文搜索，但是我们能借助搜索引擎来弥补这一缺点。当然还有其他的解决反感，比如 lunr.js 修改为 jp 则可以同时兼容英文和中文（当然效果一般），又或者接入 jieba 分词等等，但是都需要修改源码很麻烦。当然也可以用 [Digital Garden自定义组件](https://www.gachi.cn/%E8%BD%AF%E4%BB%B6%E4%BD%BF%E7%94%A8/obsidian/Digital%20Garden%E8%87%AA%E5%AE%9A%E4%B9%89%E7%BB%84%E4%BB%B6/) 去添加自定义的搜索组件，但是难度相对较大，我又很懒。  
在 dataview 和 dataviewjs 上使用警告块会造成渲染错误  
路径渲染错误 bug  
经过测试，需要在文章上传好后再更新带有 dateview 的页面，如果在文章上传之前更新 welcome，则会因为构建仓库没有这篇文章而路径渲染错误。严格来说这不是 BUG  
关于大陆访问无法加载局部关系图的问题：[Digital Garden国内访问大框问题](https://www.gachi.cn/%E8%BD%AF%E4%BB%B6%E4%BD%BF%E7%94%A8/obsidian/Digital%20Garden%E5%9B%BD%E5%86%85%E8%AE%BF%E9%97%AE%E5%A4%A7%E6%A1%86%E9%97%AE%E9%A2%98/)
## Online Resources
[^1]: [发布方案](https://www.gachi.cn/%E8%BD%AF%E4%BB%B6%E4%BD%BF%E7%94%A8/obsidian/%E5%8F%91%E5%B8%83%E6%96%B9%E6%A1%88/)
