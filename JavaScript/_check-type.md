# JavaScript(数据)类型检测
## 基本类型
### typeof {varname}: string
number,string,boolean,object,undefined, function, symbol

- typeof null === 'object', var === null 直接判断
- typeof NaN === 'number',isNaN()判断, 或者 var !== var
- undefined === void 0
- typeof 未声明变量不报错,typeof 未赋值变量返回undefined
- set/weakSet,map/weakMap

### Object.prototype.toString.call(var): string
'[object Undefined|Null|Boolean|Number|String|Object|Array|Function|Date|RegExp|Error|Arguments]'

可以检测内置数据类型,注意首字母大写

### var.constructor: function
Number | String | Array | Object | Boolean | Function

null和undefined无此属性

## 数组检测
`typeof arr === 'object'`
### Array.isArray(arr): bool 

## 原型检测

### object instanceof className/contrucotr: bool
检测对象的原型是否在构造函数的原型上

#### 原型继承关系(__proto__)

## 属性检测
### key in object: bool
### object.hasOwnProperty(key): bool

## browser
### window
`var && var === var.window`

### document
`var && var.nodeType === 9`
