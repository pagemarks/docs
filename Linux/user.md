# user
who: 当前系统登录的用户

whoami: 显示当前使用用户

groupadd: 新建用户组.后面跟用户组名参数.须root权限.

useradd: 新建用户并加入相关组.
	{username}
		eg: sudo useradd -G groupname username
passwd {password}
更改密码, 当前密码 两次新密码
	
usermod: 修改已有账户

chown: 改变文件所有权

chgrp: 更改文件的群组权限.
	   eg: sudo chgrp workgroup work/

chmod: 更改目录的权限.
	   eg: sudo chmod g+rwx work/    # g当前用户组
	       sudo chmod o-rwx work/    # o其他用户
	
/etc/passwd
/etc/group
/etc/shadow
