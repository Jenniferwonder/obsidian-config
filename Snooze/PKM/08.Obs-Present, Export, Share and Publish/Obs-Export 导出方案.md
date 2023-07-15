---
Title: Obs-Export 导出方案
tags: PKM
DateStarted: 2023-04-19
DateModified: 2023-05-27
status: null
Progress: NaN%
---
# Obs-Export 导出方案
## Metadata
### Relationships
- Topic:: [[PKM]]
- Up:: [[08.Obs-Present, Export, Share and Publish]]
- Related:: [[pandoc如何使用自定义样式导出docx文档_pandoc自定义docx样式_coderFY的博客-CSDN博客]], [[Obs-Image Import and Resize]]
- Jumps:: [[Obs-Publish 发布方案]]
## Highlights

```ad-info
Pandoc 导出文件夹为：`E:\BaiduSyncdisk\ExportFromJENNote`
```

### Plugins Required/ Available
1. Obsidian Link Converter ^hvep2r
2. Pandoc Plugin
	- 支持多种格式导出笔记
3. Pandoc-Crossref
4. Enhancing Export
### Obsidian Wiki 链接转换
1. Convert Links to Markdown > ![[Obs-Export 导出方案#^hvep2r]]
	- ! 或许只针对 Markdown 格式有效，导出为 word，图片仍无法显示
### 图片导出注意事项
##### 2. Imgur Plugin
- ? 自动上传图片，生成图片链接？
- 可自动上传图片至 Imgur🟡
##### 3. 导出 Word 与 Markdown (Typora) 兼容问题
- 导出 Word/ Markdown，将 Wiki 路径改为相对路径
	- Before 
		- `![[How to Read a Book-Four Steps-1.png|25]]`
		- ![[How to Read a Book-Four Steps-1.png|250]] 
	- After
		- `![[zz-assets/How to Read a Book-Four Steps-1.png|250]]`
		- ![[zz-assets/How to Read a Book-Four Steps-1.png|250]] 


## Online Resources
[^1]: [Obsidian Tutorial for Academic Writing | by Leonardo Castorina | Better Humans](https://betterhumans.pub/obsidian-tutorial-for-academic-writing-87b038060522)