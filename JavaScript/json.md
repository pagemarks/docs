# JSON
- NaN,Infinity,-Infinity 转换为null
- 日期对象序列化调用Date.toJSON()
- 函数,RegExp,Error undefined不能序列化及还原

### JSON.stringify(object ,replacer? ,space?)
只序列化对象可枚举的自有属性.不能序列化的属性,省略掉

- replacer 
  * 是字符串数组,包含序列化要处理的对象的属性名.
  * 是函数, 对对象调用一次,然后对对象中的每个属性各调用一次,每次传递两个参数,键和值.如果忽略某个键就返回undefined,否则返回指定的值.
- space最多十个,可为字符串值
- 数组元素不能删除,返回null

JSON.parse(string, replacer?)
	replace(key, val)<br>
		顺序遍历<br>
		先里后外(递归<br>
		this指向当前属性对象<

#### 与对象数组区别
- 属性必须用双引号
- 最后一个属性后不能有逗号
- 数值禁止出现前置0,stringify忽略,parse error
- 小数点后,至少要有一位数字
