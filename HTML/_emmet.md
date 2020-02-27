# emmet语法

## 语法
### Child: >
nav>ul>li
```html
<nav>
    <ul>
        <li></li>
    </ul>
</nav>
```

### Sibling: +
div+p+bq
```html
<div></div>
<p></p>
<blockquote></blockquote>
```

### Climb-up: ^
div+div>p>span+em^bq
```html
<div></div>
<div>
    <p><span></span><em></em></p>
    <blockquote></blockquote>
</div>
```

div+div>p>span+em^^bq
```html
<div></div>
<div>
    <p><span></span><em></em></p>
</div>
<blockquote></blockquote>
```
### Grouping: ()
div>(header>ul>li*2>a)+footer>p
```html
<div>
    <header>
        <ul>
            <li><a href=""></a></li>
            <li><a href=""></a></li>
        </ul>
    </header>
    <footer>
        <p></p>
    </footer>
</div>
```

### Multiplication: *
ul>li*5
```html
<ul>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
</ul>
```

### Item numbering: $
ul>li.item$*5
```html
<ul>
    <li class="item1"></li>
    <li class="item2"></li>
    <li class="item3"></li>
    <li class="item4"></li>
    <li class="item5"></li>
</ul>
```

h$[title=item$]{Header $}*3
```html
<h1 title="item1">Header 1</h1>
<h2 title="item2">Header 2</h2>
<h3 title="item3">Header 3</h3>
```

ul>li.item$$$*5
```html
<ul>
    <li class="item001"></li>
    <li class="item002"></li>
    <li class="item003"></li>
    <li class="item004"></li>
    <li class="item005"></li>
</ul>
```

ul>li.item$@-*5
```html
<ul>
    <li class="item5"></li>
    <li class="item4"></li>
    <li class="item3"></li>
    <li class="item2"></li>
    <li class="item1"></li>
</ul>
```

ul>li.item$@3*5
```html
<ul>
    <li class="item3"></li>
    <li class="item4"></li>
    <li class="item5"></li>
    <li class="item6"></li>
    <li class="item7"></li>
</ul>
```

### ID and CLASS attributes
#header
```html
<div id="header"></div>
```

.title
```html
<div class="title"></div>
```

form#search.wide
```html
<form id="search" class="wide"></form>
p.class1.class2.class3
<p class="class1 class2 class3"></p>
```

### Custom attributes
p[title="Hello world"]
```html
<p title="Hello world"></p>
```
td[rowspan=2 colspan=3 title]
```html
<td rowspan="2" colspan="3" title=""></td>
```

### Text: {}
a{Click me}
```html
<a href="">Click me</a>
```

p>{Click }+a{here}+{ to continue}
```html
<p>Click <a href="">here</a> to continue</p>
```

更多html与css简写,详见官方文档: https://docs.emmet.io/cheat-sheet/
