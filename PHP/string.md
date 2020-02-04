# string

## 语法
### 四种表达式
- 单引号,变量不解析
- 双引号,变量会被解析
- heredoc
- nowdoc

### heredoc
<<<后跟id符,然后换行,字符本身,最后用前面定义的标识符结束.<br>
结束标识符,需在第一列.后面的分号,不能有其他字符.标识符同变量规则无$.
```php
<<<{id}
...
id;
```

### nowdoc
heredoc类似双引号,nowdoc类似于单引号,不解析字符串中的变量和表达式.<br>
开始标识符用单引号括起来

### {}
双引号中支持简单表达式/对象属性/数组元素

### 转义字符
\后跟特殊字符,如\, n, r, t, v, e, f, $, ",x[0-9A-Fa-f]{1,2}

### 数组索引访问修改


## 运算符
### .
连接两个字符串类型为一个字符串

## 转换成字符串
- (string)
- strval()
- settype()
- 自动转换,echo/print/.

## 相关函数
### 格式化类
### addslashes($string): string / stripslashes
为数据库查询语句等需要在某些字符前加反斜线. stripslashes去掉相关反斜线

### htmlspecialchars($string, $flags?, $encoding?, $double_encode ?): string / htmlspecialchars_decode($string, $flag)
转义html中的实体字符. \&amp;,\&gt;

- $flags = ENT_COMPAT | ENT_HTML401,处理转义细节
- $encoding = ini_get('default_charset'),设置字符集, utf-8
- $double_encode = true, 不转换已有的实体.

### nl2br() / br2nl
换行符转换为HTML换行标记

### bin2hex($string): string / hex2bin

### trim($string): string / ltirm / rtrim 

### strtolower($string): string / strtoupper
字符串大小写转换.

### ucfirst / lcfirst

### ucwords / lcwords



### 输出类
### echo (...$args): void: <?=$var?>
### print($var): int, 可省略(),始终返回1
### printf($string, $args,)
### sprintf($string, ...$args): string

### 截取类

### 查找类

### 统计类








https://www.php.net/manual/zh/language.types.string.php
https://www.php.net/manual/zh/ref.strings.php
