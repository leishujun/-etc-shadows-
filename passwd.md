
# **/etc/passwd的格式**
```
wang:x:1000:1000:wang:/home/wang:/bin/bash
```
wang：用户

x：加密方式和密码

1000：UID

1000：GID

wang：描述字段，用于描述账户的一些个人信息使用chfn可以修改，使用finger可以查看

/home/wang：用户的家目录

/bin/bash：用户使用的shell语言类型，nologin的一般是系统的后台进程，使用nologin的都是不允许登陆的，使用chsh  -s   /sbin/nologin  用户名  这个命令会让用户无法登陆