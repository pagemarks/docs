# set 与 map

Set
非重复值的有序集合,数组去重,区别数据类型.
对象模拟,不能区分转换.

let set = new Set([array | iterable])  // 结合Array.of,数组去重

size
返回set集合中元素的个数

add(val)

has(val) :bool

delete()

clear()

forEach(function(key, val, set){} [, this]) key/value同值

扩展运算符可以将set直接转换为数组.

Weak Set
只能储存对象,对象被回收,则Weak Set中的对象会直接释放.
对于WeakSet的实例,只要调用add(),has(),delete()方法时,传入了非对象的参数,就会抛出错误.
WeakSet不可迭代,没有任何编程手段可用于判断WeakSet的内容
WeakSet没有forEach()方法,size属性

Map
键的比较使用的Object.is() 因此 5 和 '5'区别于传统对象是不同key
set(key, value)

get(key)

has(key)

delete(key)

clear()

size

forEach((key, val, map)=>{}, this?)  遍历为添加顺序

let map = new Map([[key, val],[key, val],...])

Weak Map 键必须是对象
get()
set()
has()
delete()
