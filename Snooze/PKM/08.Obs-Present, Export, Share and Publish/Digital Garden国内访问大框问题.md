---
Title: Digital Garden国内访问大框问题
Topic: 
tags: 
DateStarted: 2023-05-10
DateModified: 2023-05-19
---


[Digital Garden国内访问大框问题](https://www.gachi.cn/%E8%BD%AF%E4%BB%B6%E4%BD%BF%E7%94%A8/obsidian/Digital%20Garden%E5%9B%BD%E5%86%85%E8%AE%BF%E9%97%AE%E5%A4%A7%E6%A1%86%E9%97%AE%E9%A2%98/)

## 无法加载文件关系图

因为 cdn.jsdelivr.net 在国内已经无法使用，而 Digital Garden 在 vercel 的构建仓库中默认使用的确实 cdn.jsdelivr.net。导致在国内访问的时候无法加载对应 js，则会出现下图的问题。  
![image.png](http://cdn-ob-pic.hningyun.com/simp/202305022222282.png-shoushen)  
这个问题一开始也困扰了我一段时间，毕竟如果关闭局部关系图的展示那还叫数字花园吗？而且我自己访问其实并不会出现这个问题，直到我在看到了 cdn.jsdelivr.net 后。。。

## 替换 Cdn 解决问题

首先将托管仓库拉到本地（不会拉就百度，教程都挺详细的）

需要替换的文件目录：

1. `src\site\_includes\components\pageheader.njk`
2. `src\site\_includes\components\timestamps.njk`

将 `cdn.jsdelivr.net` 使用 `ctrl+h` 替换为 `fastly.jsdelivr.net`,下图是我替换后的结果  
![image.png](http://cdn-ob-pic.hningyun.com/simp/202305022231339.png-shoushen)

commit 这次修改，然后 push 到远程仓库。等待 vercel 构建完成后访问，应该就没问题了

![image.png](http://cdn-ob-pic.hningyun.com/simp/202305022233765.png-shoushen)

![image.png](http://cdn-ob-pic.hningyun.com/simp/202305022233502.png-shoushen)

我已经向作者提交了 issue，在作者采纳之前可以作为临时补救方法 2023 年 5 月 2 日 22:36:07