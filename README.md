# free-libc
请注意，free-libc并不支持源代码.c级别的调试，如果想获取源代码.c级别调试能力，请参考我的gfree-libc项目。
================================
Please note that free-libc does not support source code. C level debugging, if you want to get the source code. C level debugging capabilities, please refer to my gfree-libc project.
=================================
gfree-libc---》https://github.com/dsyzy/gfree-libc

Do you want the program to use the specified libc version?Come on then!
Warning, please backup the source before use！！！！
=================================
使用前请先备份文件！！！！
=================================
当前支持的libc版本如下/The currently supported libc version is shown below.
=================================
-2.24-3ubuntu1_amd64

-2.24-3ubuntu1_i386

-2.27-3ubuntu1_amd64

-2.27-3ubuntu1_i386

-2.28-0ubuntu1_amd64

-2.28-0ubuntu1_i386

-2.29-0ubuntu2_amd64

-2.29-0ubuntu2_i386

How to install?
=================================
1.git clone https://github.com/dsyzy/free-libc.git

2.cd free-libc

3.sudo sh ./install.sh



怎么使用/How to use?
=================================
测试文件是PWN，测试libc版本是2.27/The test file is PWN，the test libc is 2.27-libc.so
=================================
如果不指定使用当前目录libc/If there is no local libc file,then:
=================================
clibc PWN 2.27

clibc是指令 PWN是需要更改的程序 2.27是libc版本

如果指定使用当前目录libc/If there is a local libc file,then:
=================================
clibc PWN 2.27 2.27-libc.so

clibc是指令 PWN是需要更改的程序 2.27是libc版本 2.27-libc.so是自自指定加载的libc文件


如果你想添加你想要的版本/How to add the version you want:
=================================
1,Gets the libc file package,such as 2.30-ubuntu-libc

2,If it's a 32-bit libc library:sudo mv 2.30-ubuntu-libc /usr/lib/freelibs/i386

3,If it's a 64-bit libc library:sudo mv 2.30-ubuntu-libc /usr/lib/freelibs/amd64


created by freedom
