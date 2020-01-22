# storage

sessionStorage
有效期为回话时间内,需关闭浏览器,关闭tab再打开网页会存在

localStorage
永久有效,需手动清理

方法
getItem(name)

setItem(name, value)
value为字符串

removeItem(name)
删除相关name储存值

clear()
清理目前网站下所有的存储设置

事件
window.addEventListener('storage',callback(e).false)
event
	key
	oldValue
	newValue
	url
	storageArea
	
-一般一个域限制5M
