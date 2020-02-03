# TypeScript
类型约束 + 经典类 + 命名空间 + 模块

## 变量申明
### 基本类型
let varname: TYPE = value;
TYPE: boolean | number | string | any | null | undefined | object | Date

- object 可含null

### 类型转换
let length: number = (<string>value).length / (value as string).length

### 数组类型
number[] | Array<TYPE>

### 固定数组
let arr: [string, number]

### 枚举类型
enum Color = {Red = 1, Green, Blue}
let c: Color = Color.Green
let colorName: string = Color[2]

默认从0开始,可以赋值改变其值.可以通过值反向获取名

## 函数
### 返回值
function fnname(args): void {...}

never: 函数无返回值或抛出一个错误

### 变量限制
function fnname(arg: TYPE = default): TYPE {...}

## 接口限制
interface MapVals {
	key1: TYPE,
	key2: TYPE,
	key3?: TYPE,
	readonly key4: TYPE
}

interface fnType {
	(...arg: TYPE): TYPE
}
//用于函数赋值给变量

interface array {
	[index: number]: string
}
//字符串数组

function fnname(arg: MapVals) {...}

需包含interface所申明的属性字段,可超出. ?表示可选

## class
### public private protected static readonly
经典类属性/方法限制

### abstract

## 泛型

function fnname<T>(arg: T): T {
	...
} 

function fnname<T extends interface>(arg: T): T {}


- any 区别, 正则匹配单双引号

### keyof


http://www.typescriptlang.org/docs/handbook/basic-types.html
