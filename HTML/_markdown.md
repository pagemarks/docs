# markdown 语法

#{1,6} {text}: h1-h6,注意后面与文本有个空格

text: 常规段落,有换行和空格

\*{text}\* | \_text\_: *或_包裹的文本为斜展示

\*\*{text}\*\* | \_\_{text}\_\_: 两个*|_包裹的文本为加粗显示

![alt text](src): 插入图片
[text](url): 超链接

\`code\`: 代码片段

\> text: 引用

\* | \- : 无序列表,嵌套列表须用tab.li>ul>li
1\. : 有序列表,num+dot

## GitHub扩展
### 代码片段
语法高亮显示
<pre>
```{language}
....codes
```
<pre>

### 任务列表
checkbox

\- \[x\] : 已完成项
\- \[ \] : 未完成项

### 表格
--- 风格表头th和正文
<pre>
text | text 
---- | ----
text | text
<pre>

\可转译相关字符

可直接书写html相关标签


https://guides.github.com/features/mastering-markdown/

https://developer.github.com/v3/markdown/
