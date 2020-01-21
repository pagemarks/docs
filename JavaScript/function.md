# function

默认参数
在函数声明时,直接在参数后=赋值. 传参undefined会使函数使用默认值.null不使用.
可以给默认参数赋值为函数运算值,懒执行.传参不执行.
赋值可以为前面的参数名,前面参数不能访问后面的参数.暂时性死区

arguments
ES5非严格模式下,arguments会反映出具名参数变化(具名参数在函数内改变值,arguments对象相关值会跟着变化).
严格模式下,表示传参时的值.
ES6默认参数情况下,arguments表示调用传递时,实际传递的参数.

剩余参数
…args
函数只能有一个剩余参数,并且放在最后.
不能在对象字面量的setter属性中使用.(set被限定只能使用单个参数)
不参加函数的length属性.

扩展运算符
…arr
将一个数组分割,并将各个项作为分离参数传递给函数.Math.max()
let values = [1,2,3,4,5]
Math.max(…values [,arg])

属性
name: 返回函数名.
bind -> bound
Function -> anonymous
method -> method name
get name
set name
赋值函数如果具名,则返回具名名称

自定义函数属性,类似静态属性

call(context, arguments...)

apply(context, [arguments...])

bind(context, arguments)

实参与形参
arguments
functionName.length


arguments
callee: 函数
caller: 调用函数

构造函数
new.target 判断是否为undefined,new为对象值.该值不能在函数外调用

new Function(arguments, body)
在顶层作用域执行,不能访问局部变量.ES6可以使用默认参数和剩余参数

ES5严格模式禁止块级函数声明,ES6则可以.块级具名函数存在作用域提升.非严格模式下,全局声明.(向下兼容)

箭头函数
没有this,super,arguments,new.target绑定.由最靠近的非箭头函数决定
不能被使用new调用
没有原型
不能更改this
不允许重复的具名参数,传统函数在严格模式下禁止
没有自己的arguments对象,但可以访问包含它函数的arguments对象

单个参数时,可以省略括号.箭头右边的表达式会被直接计算,然后返回.
无参数时,需使用空括号表示.函数体包含多条语句时需要用{}进行包裹,并明确定义一个返回值.
如果直接返回一个对象字面量,需使用()包裹
value => value
(num1,num2) => num1+num2
空函数: ()=>{}

生成器函数

函数调用
	直接调用 [[Call]]
	对象方法
	构造函数 [[Construct]]
	call,apply

立即执行函数
(function(){})() / (function(){}())
!function(0{}()
~function(){}()
+function(){}()
-function(){}()

块级函数
非严格模式下和ES5一样


尾调优化
	尾调不能引用当前栈帧中的变量(意味该函数不能是闭包)
	进行尾调用的函数在尾调用返回结果后不能做额外操作.
	尾调用的结果作为当前函数的返回值
	
链式调用,方法返回对象
