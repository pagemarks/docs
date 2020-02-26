# console

### log(...args)
支持多个参数同时输出.<br>
也支持字符格式化功能.
- %s: string
- %d %i: int
- %f: float
- %o %O: object
- %c: css style rules: 'color: red;background:blue'
- %O like console.dir()


### error(var),trace(var),info(var),warn(var)
输出时与log样式不同,error和trace会输出调用栈

### dir(object):
输出展开对象

### dirxml(dom):
dom tree

### table(array | object):
表格形式展示,对象数组

### time(string label),timeEnd(string label):
中间包含代码运行时间统计

### count(string label):
执行次数

### assert(assertion, falseMessage...)
断言为假时,输出内容,内容设置通log参数.node.js会阻断代码运行

### group(),groupEnd():
输出层级嵌套.groupCollapsed()与group类似,不过是折叠状态

### profile(string label),profileEnd():
监控性能分析,在控制台的profiles展示

### clear():
清空控制台内容.

### trace(tagName)
调用栈分析,调用函数内
