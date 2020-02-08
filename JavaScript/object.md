# Object

## 创建对象

### 对象直接量

### new

### Object.create(proto, obj?)

## 属性
### 属性访问
- obj.key
- obj[key]: 支持变量和表达式

### 删除属性
delete obj[key]

### 属性检测
- key in obj: 检查原型链上
- obj.hasOwnProperty(key)
- obj.propertyIsEnumerable(key): 自有属性且可枚举

### 枚举属性
for key in obj

### 存取器属性
get key() {}
set key(val) {}

### 属性特性
- writable
- enumerable
- configurable
- value

### prototype
### constructor


## 方法
#### 属性类
### Object.definePeoperty(obj, desObj)
### Object.defineProperties(obj, desObjs)
desObj = {value, get(), set(), writable, enumerable, configurable}

### Object.getOwnPropertyDescriptor(obj, key): object

#### 原型类
### Object.getPrototypeOf(obj): object
### Object.


