通配符
*: 匹配多个字符
?:
.: 匹配任意字符

grep [options] pattern [file]
在文件中搜索内容.搜索内容有空格时,须加单引号.
	-i: 忽略大小写
	-v: 反向匹配
	-E: 

find: 在文件目录下查找文件.
     find [options] [path] [expression]
     eg: $ find /usr/bin/ -name zip -print

	-name: 指定文件名
	-type:  指定文件类型.
	       b: 块设备文件
	             c: 字符设备文件
	             d: 目录文件
	             f: 普通文件
	             p: 命名管道
	             l: 符号链接
        -atime: 查找使用在n天前的文件
        -mtime: 查找最后一次修改在n天前的文件.(可为负

locate: 检索数据库中搜索文件.updatedb 更新检索数据库,需要root权限

whereis: 在固定目录(/usr/bin,/usr/sbin/,/usr/share/man)中搜索
