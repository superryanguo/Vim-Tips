加密文件
==================
vim一个比较好用的功能就是对文件进行加密，而且加密的使用比较简单。

新建一个vim加密文件
-----------------------
使用vim的`-x`选项就可以加密文件。
```bash
$ vim -x encrypted-files.txt
```
如果要对文件加密会提示你输入两次密码。

打开或关闭文件加密
----------------------
要停止对一个文件加密, 可以把`key`选项设置为一个空字串
```viml
: set key= 
```
**等于号后面有一个空格**，否则无效。

通过设置`key`的值来进行加密可不是一个好主意, 因为密码会显露无遗。任何趴在你肩膀上的人都能看到你的密码。一个解决的方案是使用下面的Ex命令：
```viml
:X
```




