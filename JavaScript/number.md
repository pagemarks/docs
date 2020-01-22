# Number

## 属性
### Number.MAX_VALUE
### Number.NEGATIVE_INFINITY
### Number.POSITIVE_INFINITY
### NaN

### isNaN()

### isFinite()

### parseInt(string[, radix])
忽略字符串前面的空格,直至找到第一个非空格字符.若后续字符非数字,则停止解析,返回前面匹配的数字.可选参数控制进制

### parseFloat(string)
将字符串转换为浮点数,不识别非十进制

### toFixed(num)
根据小数点后的指定位数,将数字转换为字符串,不使用指数计数法

### toExponential(num)
使用指数计数法将数字转换为指数形式的字符串.小数前只有一位,小数点后面的数由参数指定.

### toPrecision(num)
根据指定的有效数字位数将数字转换成字符串.如果有效数字位数少于数字整数部分的位数,则转换成指数形式.


### toString(radix)

## 转换规则
- 如果是boolean值,true和false分别转换为1,0
- 如果是数字,只是简单的传入与返回
- 如果是null,返回0
- 如果是undefined,返回NaN
- 如果是字符串
  * 如果只含数字,将其转换为十进制,前置0会被忽略
  * 如果包含浮点数格式,则转换为对应的浮点数值
  * 如果是有效的十六进制格式,则转换为对应的十进制整数值
  * 如果是空的,则将其转换为0
  * 其他形式转换为NaN
- 如果是对象,则调用对象的valueOf方法,按前面规则转换.如果转换值是NaN.则调用toString方法按上面规则处理.

## ES6 新增
### Number.isInteger()

### Number.isSafeInteger()

### Number.isNaN()

### Number.isFinite()
