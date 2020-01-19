- doctype
- html
- head: 设置包含关于文档自身的信息,它们不会被显示在屏幕上
    - base: 为文档中所有链接指定一个基础URL,把网页内链接变得更简短易维护.
        * href: 指定一个URL,用作文档中的链接的基础URL
    - link: 定义两个链接在一起的文档之间的关系.它最常用于把外部样式表链接进当前文档.
        * charset: 设置所链接的文档使用的字符集
        * href: 指向所链接的文档URL
        * media: 所链接的文档应用于哪种媒介
            - all:
            - print:
            - screen:
            - projection:
            - speech:
        * rel: 定义所链接到的文档与当前文档之间的关系.
        * rev: 定义当前文档与所链接到的文档之间的关系
        * type: 指定目标URL的MIME类型
    - meta: 提供文档的信息
        * name: 为文档赋予额外的信息.该属性的值来自content属性.常见名称包括author,keywords,description
        * content: 设置name相关值
        * http-euiv:
    - script: 为文档引入脚本文件
        * type: text/javascript
        * charset:
        * defer:
        * src:
        * async:
    - style: 为文档引入样式文件
        * type
        * media:
        * src:
    - title: 为文档提供一个标题
- body
    - p: 段落,表达一种看法/主题的一个或多个句子
    - h{1~6}: 标题.提供6个级别的标题元素,重要性从上至下排列.
    - blockquote: 标明一段长引文,如书中的一段文字或评论中的推荐词.
        * cite: 引文的原始来源URL
    - address: 当前文档负责的人或组织的联系信息
    - pre: 保留文本中的空白和换行,使其原样保留.默认合并空白符
    - ul: 无序列表
    - ol: 有序列表
    - li: 定义列表项
    - dl: 定义列表
    - dt: 术语
    - dd: 说明
    - em: 强调一个词或短语
    - strong: 比em强调重
    - cite: 标明对某一资源的引用,可以是书,影片标题等
    - q: 标记前端的行内引文.
        * cite:
    - dfn: 表示术语的定义实例
    - abbr: 缩写
        * title
    - del: 标记修改文档中被删除的文本
    - ins: 标记插入的文本
        * cite:
        * datetime:
    - bdo: 重置一段文本的方向
        * dir:
    - code: 标明一段代码
    - kbd: 标明用户键入的命令文本
    - samp: 标明程序的输出样例
    - var: 标明编程变量或参数
    - i:
    - b:
    - sup:
    - sub:

    - br: 手动换行
    - hr: 创建一条横线
    - div: 创建一个逻辑部分
    - span:
    - object: 嵌入一个外部的文件或某种类型的媒体
    - param: 设置object相关参数
        * name
        * type
        * value
    - map:
    - area: 
    - img : (图片文件格式专题介绍)
        * src
        * alt
        * width
        * height
        * ismap
        * usemap
        * longdesc
    - a:
        * href:
        * id
    - table
    - thead
    - tbody
    - tfoot
    - tr
    - th
    - td
        * rowspan
        * colspan
        * scope: row | col
    - caption
    - colgroup
    - col
    - form
        * action
        * accept
        * enctype: application/x-www-form-urlencoded, multipart/form-data
    - input
        * type
    - label
    - button
        * type
    - select
    - option
    - optgroup
    - textarea
    - fieldset
    - legend

相关标签样式,表格/表单可链接至css相关部分

