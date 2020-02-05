# 字符串

## 语法
- 单引号
- 双引号
- 模板字符
- String转换
- 转义字符

## 属性

### String.prototype
对象原型，可扩展字符串相关方法和属性

### length： int
返回一个字符串的长度

## 方法
### 转换类
### String.fromCharCode(...num): string
将对应的unicode编码转换(映射)为字符. num < 65535

### String.fromCharPoint(...num): string
多字节字符支持,表情符

### 访问类
### charAt(pos=0): string
返回字符串自定位置的字符, 从0开始索引.超出索引返回为空

### charCodeAt(pos): number
返回指定位置字符的unicode值

### charCodePointAt(pos=0): number
支持多字节,表情符

### concat(...string): string
多个字符拼接为一个字符

### endswith(string, length?): bool
判断字符串是否以给定的字符结尾,length可限定字符串的长度.

### includes(string, pos = 0): bool
判断字符串是否包含给定参数的字符串,pos可设置搜索起始位置.indexOf()优化

### indexOf(string, pos=0): int
查找给定字符在字符串中出现的初始位置,pos可设置搜索位置

### lastIndexOf(string, pos=0): int
反向查找


https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/String
