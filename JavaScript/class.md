# class
class className {
	contructor() {
	// ES5 构造函数
	}
	
	method() {      //ES5 ctor.prototype
	}
	
	static 
}

typeof className === 'function'

类声明不会提升,与let类似
类声明代码会自动在严格模式下运行,无法退出严格模式
类的所有方法都是不可枚举的,可以通过Object.defineProperty()修改
类的所有方法没有[[construct]], 所以不能new
调用类构造器时不使用new,会抛出错误,
试图在类的方法内部重写类名,会报错误

和函数一样,也支持表达式形式,可以作为函数参数传入
支持访问器属性设置.
支持动态计算方法名
方法支持生成器写法

继承
extends
super(args...) 只能在派生类中使用
静态方法 自动继承
覆写父类方法,可以super.methods 调用
