1。停止mysql服务。//打开命令行窗口，停止mysql服务： Net stop mysql

　　2。启动mysql，一般到mysql的安装路径，，找到 mysqld-nt.exe

　　执行：mysqld-nt --skip-grant-tables 当前窗口将会停止。

　　3。另外打开一个命令行窗口，进入MYSQL的安装位置下BIN目录，运行mysql

　　4。输入如下命令：

　　>use mysql

　　>update user set password=password("new_password") where user="root";

　　>flush privileges;

　　>exit

　　6。用Ctrl+Alt+Del，找到mysqld-nt的进程杀掉它，在重新启动mysql-nt服务，就可以用新密码登录了
