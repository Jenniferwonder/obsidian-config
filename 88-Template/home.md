
```ad-blank
- [[00-Tips|使用技巧]]
- `button-inbox`
- [[示例库移植说明|移植说明]]
- [[🔑Dataview教程]]
- [[电影看板|影视看板]]
```

````ad-grid
> [!profile-card|cards]  `button-refreshhomepage1`
> ***快乐摸鱼又一天***
> **瞅瞅你的笔记写了多少篇**
>>[!profile-card-inf|noborder]
>>```dataviewjs
>>let nofold = '!"88-Template"'
>>let ftMd = dv.pages("").file.sort(t => t.cday)[0]
>>let total = parseInt([new Date() - ftMd.ctime] / (60*60*24*1000))
>>let allFile = dv.pages(nofold).file
>>dv.paragraph(`
>>>[!item|noborder] [[echarts-笔记动态显示-分布|${total}]]
>>> Ob天数
>>
>>>[!item|noborder] [${allFile.length}](obsidian://advanced-uri?commandid=obsidian-better-command-palette%253Aopen-better-commmand-palette-file-search)
>>> 文档
>>
>>>[!item|noborder] [[文件夹所有标签|${allFile.etags.distinct().length}]]
>>> 标签
>>
>>>[!item|noborder] [[任务卡片-dataview 任务查询举例#所有未完成的任务|${allFile.tasks.length}]]
>>> 事项`)
>>```

>[!profile-card-inf|noborder]
> ```dataviewjs
>let nofold = '!"88-Template" and !"99-Attachment" and !"50-Inbox" and #book or #Movie'
>let reg =/!\[[^\]]*\]\((?<=\!\[.*\]\()(.*(jpg|jpeg|bmp|gif|png|JPG|JPEG|BMP|GIF|PNG|WebP).*)(?=\))\)/ //匹配网络链接图片
>let files = dv.pages(nofold).file
>const arr = files.map(async (file) => {
>const sampleTFile = this.app.vault.getAbstractFileByPath(file.path);
>const content = await this.app.vault.cachedRead(sampleTFile); 
>const links = content.match(reg);
>if (links) 
>{let res ={'file':file.path,'link':links[1]}
>return res}
>})
>Promise.all(arr).then(
>values => 
>{
>let flatvalues =values.filter(Boolean).flat()
>const random = Math.floor(Math.random() * (flatvalues.length - 1))
>dv.paragraph(`[![image|220](${flatvalues[random].link})](obsidian://open?file=${encodeURIComponent(flatvalues[random].file)})`)
>}
>)
>```
%%调用词霸的每日海报%%
%%数据位于.obsidian/.diary-stats%%
```dataviewjs
let history = Object.assign(JSON.parse(await app.vault.adapter.read(".obsidian/.diary-stats")));
let today = moment().format("YYYY-MM-DD");
if (history.hasOwnProperty(today))
{
let posters=history[today].posters;
dv.paragraph(posters);
}
```
````

%%便签板块%%
%%可通过侧边栏主页便签按钮快捷更改便签内容%%
---

````ad-flex
%%notice1%%
> [!stickies3]
> #### 倒计时
>> 今年已过去 <%+* tR+= moment().diff(tp.date.now("YYYY-1-1"), "days") %> 天
>> 
>> 距春节还有<%+* let edate = moment("2022-02-01", "yyyy-MM-DD"); let from = moment().startOf('day'); edate.diff(from, "days") >= 0 ? tR += edate.diff(from, "days") : tR += edate.add(1, "year").diff(from, "days") %> 天

%%notice2%%
> [!stickies3|blue]
>```dataviewjs
async function removeMarkdown (text) {
let excludeComments= true;
let excludeCode= true; 
let plaintext = text;
if (excludeComments) {plaintext = plaintext.replace(/<!--.*?-->/sg, "").replace(/%%.*?%%/sg, "");}
if (excludeCode) {plaintext = plaintext.replace(/```([\s\S]*)```[\s]*/g, "");}plaintext = plaintext.replace(/`\$?=[^`]+`/g, "").replace(/^---\n.*?\n---\n/s, "").replace(/!?\[(.+)\]\(.+\)/g, "$1").replace(/\*|_|\[\[|\]\]|\||==|~~|---|#|> |`/g, ""); return plaintext;}
async function getradomnote (files) {
const random = Math.floor(Math.random() * (files.length - 1));
const randomNote = files[random];
dv.paragraph(randomNote.link);
const sampleTFile = app.vault.getAbstractFileByPath(randomNote.path);
const contents = await app.vault.cachedRead(sampleTFile); 
return contents;}
let reg=/[\u4e00-\u9fa5]/
let nofold = '!"88-Template" and !"99-Attachment" and !"50-Inbox" and !"20-Diary"';
let files = dv.pages(nofold).file;
let content =await getradomnote(files);
let clean= await removeMarkdown(content);
let lines = clean?.split("\n").filter(line => line.match(reg));
const randomline = Math.floor(Math.random() * (lines.length - 1));
lines = lines[randomline]?.replace(/(\r|\n|#|-|\*|\t|\>)/gi,"").substr(0,80) + '...';
dv.span(lines);
>```

%%notice3%%
> [!stickies3|pink]
> #### 每日一句
> ```dataviewjs
 let history = Object.assign(JSON.parse(await app.vault.adapter.read(".obsidian/.diary-stats")));
 let today = moment().format("YYYY-MM-DD");
 if (history.hasOwnProperty(today))
 {
 let quotes=history[today].quotes;
 dv.el("blockquote", quotes);
 }
> ```

%%notice4%%
> [!stickies3|green]
> ### 💌
> 开启美好的一天
````

---

````ad-flex
```ad-note
title: 🤔 快速导航
color: 178,155,64
> “Quick Access”
-  `button-richeng`

-  `button-kanban`

- `button-suibi2`

- `button-renwu2`

- 📆 `$= '[[日记统计#'+ moment().format("YYYY-MM") +'|当月日记]]'`

```
```ad-note
title: 😏 功能
color: 99,188,76
> “Common actions”
- Ⓜ️ [生成MOC](obsidian://advanced-uri?commandid=templater-obsidian%253A88-Template%252Ftp_foldermoc-Include-subfolders.md)

- 📚 [豆瓣读书](obsidian://advanced-uri?commandid=quickadd%253Achoice%253A19402f67-f691-4b0f-9975-f8203e74be96)

- 🎞️ [豆瓣电影](obsidian://advanced-uri?commandid=quickadd%253Achoice%253Aaabcb6ad-5faa-45fb-a713-deddc27bc384)

- 💠 [[随机显示文档中的图片和文字|随机漫游]]

```

```ad-note
title: 🥰 阅读笔记
color: 178,22,164
> “Media”

- 💬 [[微信读书清单|微信阅读]]

- 📑 [[图书阅读清单(dv)|图书馆]]

- 👁 [[电影看板]]

- 🛹[[可以编辑的dv表格|资料维护]]

```
```ad-note
title: 🤩 帮助教程
color: 139,65,06
> “Tutorials”

- 🚩 [Cuman的B站](https://b23.tv/2Uqt2dn)

- 🥑 [[🥑Blue Topaz Themes Tips|主题TIPS]]

- 🇲🇩 [[MarkDown教程 Obsidian版 2022.4.22|MD超级教程]]

- [[🔑Dataview教程]]

- 💾 [[77-Example|示例库]]

```
````



![[从这开始#MOC 另一种样式]]

![[从这开始#最近编辑]]

![[通过下拉框检索文件示例]]

![[项目追踪（完成的字数和任务）#选择需要跟踪的项目]]

---
