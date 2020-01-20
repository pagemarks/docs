# flex 弹性布局
## containor
```css
display: flex | inline-flex
```

`子元素的float/clear/vertical-align`将失效

### flex-direction
- row
- row-reserve
- column
- column-reserve

### flex-wrap
- nowrap
- wrap
- wrap-reserve

### flex-flow: {flex-direction} {flex-wrap}

### justify-content
- flex-start
- flex-end 
- center
- space-between
- space-around

### align-items
- flex-start
- flex-end
- baseline
- center
- stretch

### align-content
多行时对齐方式

- flex-start
- flex-end
- center
- space-between
- space-around
- stretch

## item
### order: int

### flex-grow
### flex-shrink
### flex-basis: <length> | auto
### flex: <flex-grow> <flex-shrink> <flex-basis> | none
### align-self
- auto
- flex-start
- flex end 
- center
- baseline
- stretch

* http://www.ruanyifeng.com/blog/2015/07/flex-grammar.html

