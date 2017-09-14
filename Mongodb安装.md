# Mongodb 的安装
###Ubuntu下
在linux下，特别是Ubuntu下，是比较简单的，直接使用命令

`sudo apt-get install mongodb`

便可以安装

查看mongodb的版本 `mongo -version`

启动和关闭 

`service mongodb start`

`service mongodb stop`

参考资料 http://blog.csdn.net/flyfish111222/article/details/51886787

### 一般方法
官网下载安装包，然后解压，移动到相关目录，如：`mv  mongodb-linux-x86_64-3.0.6/ /usr/local/mongodb`

将可执行文件添加到PATH目录 `export PATH=<mongodb-install-directory>/bin:$PATH`

\<mongodb-install-directory> 为你 MongoDB 的安装路径。如本文的 /usr/local/mongodb

还要创建数据文件夹 `mkdir -p /data/db`，可以创建在其他地方，不过后面连接的时候需要指定


命令行运行 Mongodb服务

``注意：如果你的数据库目录不是/data/db，可以通过 --dbpath 来指定。``

到bin目录，`cd/usr/local/mongodb/bin`,

`./mongodb`,开启服务，有时候因为data文件夹的权限，或者是端口之前以及开过没关，会造成报错，相应的杀进程开权限就好了

进入MongoDB后台管理

同样到bin目录，`./mongo`,就能进入