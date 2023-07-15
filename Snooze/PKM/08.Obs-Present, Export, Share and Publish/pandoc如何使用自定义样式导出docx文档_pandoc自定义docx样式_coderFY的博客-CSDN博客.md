---
Title: pandoc如何使用自定义样式导出docx文档_pandoc自定义docx样式_coderFY的博客-CSDN博客
Topic: null
Type: null
tags:
  - Resonance
  - PKM
DateStarted: 2023-05-19
DateModified: null
Progress: NaN%
---
## Metadata
### Source
Author:: 成就一亿技术人! 
SourceURL:: https://blog.csdn.net/waitting_in_love/article/details/126598266?spm=1001.2101.3001.6650.1&utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7ECTRLIST%7ERate-1-126598266-blog-128335420.235%5Ev36%5Epc_relevant_anti_vip_base&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7ECTRLIST%7ERate-1-126598266-blog-128335420.235%5Ev36%5Epc_relevant_anti_vip_base&utm_relevant_index=2

### Relationships

## Highlights

## Contents

![](https://csdnimg.cn/release/blogv2/dist/pc/img/original.png)

版权声明：本文为博主原创文章，遵循 [CC 4.0 BY-SA](http://creativecommons.org/licenses/by-sa/4.0/) 版权协议，转载请附上原文出处链接和本声明。

### 目录

-   -   [1.导出默认样式文件](https://blog.csdn.net/waitting_in_love/article/details/126598266?spm=1001.2101.3001.6650.1&utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7ECTRLIST%7ERate-1-126598266-blog-128335420.235%5Ev36%5Epc_relevant_anti_vip_base&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7ECTRLIST%7ERate-1-126598266-blog-128335420.235%5Ev36%5Epc_relevant_anti_vip_base&utm_relevant_index=2#1_3)
    -   [2.修改样式文件](https://blog.csdn.net/waitting_in_love/article/details/126598266?spm=1001.2101.3001.6650.1&utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7ECTRLIST%7ERate-1-126598266-blog-128335420.235%5Ev36%5Epc_relevant_anti_vip_base&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7ECTRLIST%7ERate-1-126598266-blog-128335420.235%5Ev36%5Epc_relevant_anti_vip_base&utm_relevant_index=2#2_11)
    -   [3.使用自定义的样式导出markdown](https://blog.csdn.net/waitting_in_love/article/details/126598266?spm=1001.2101.3001.6650.1&utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7ECTRLIST%7ERate-1-126598266-blog-128335420.235%5Ev36%5Epc_relevant_anti_vip_base&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7ECTRLIST%7ERate-1-126598266-blog-128335420.235%5Ev36%5Epc_relevant_anti_vip_base&utm_relevant_index=2#3markdown_19)

pandoc是一个方便的文档格式转换工具，其中一个功能是将markdown文件转换为docx文件，但是它是使用的自带样式，如果需要自己规定样式就需要提供一个样式文件。

## 1.导出默认样式文件

```
 pandoc -o custom-reference.docx --print-default-data-file reference.docx
```

这会在终端当前所在的文件夹下导出pandoc默认的docx导出格式。

## 2.修改样式文件

使用Microsoft Word 或者WPS修改样式文件，注意，**此处不是修改文档中内容的格式，而是修改文档的预设样式**：

![image-20220830101100554](https://img-blog.csdnimg.cn/img_convert/fb5b95646bd148c17491e1e364d29e23.png)

刚开始不理解来来回回弄了好几次。

## 3.使用自定义的样式导出markdown

```
pandoc -s markdown.md --reference-doc custom-reference.docx -o m.docx
```

其中markdown.md是现有文件，m.docx是导出后的文件名。  
或者使用typora集成好的功能，直接设置样式文件地址进行一键导出  
![在这里插入图片描述](https://img-blog.csdnimg.cn/344b34961b01427695687a658c6e18b3.png)