# Zeppelin

## Zeppelin mac 安装步骤：
1.官网下载二进制文件进行安装，zeppelin-0.8.1-bin-all.tgz, 
下载链接https://zeppelin.apache.org/download.html

为了保证系统正常启动，确保的 zeppelin.server.port 属性的端口不被占用，默认是8080。

2.解压，进入Zeppelin 安装目录的bin文件夹下，使用以下命令启动进程：

./zeppelin-daemon.sh start

若需要停止，可以使用以下命令停止进程：

./zeppelin-daemon.sh stop

3.Check out the Zeppelin web notebook at http://localhost:8080


## Zeppelin windows 安装步骤：
1.下载安装包并解压

2.Zeppelin在不用做任何配置修改的情况下即可正常启动。进入Zeppelin的bin目录，执行以下命令:zeppelin.cmd

3.Zeppelin启动失败原因分析及解决
问题现象：执行zeppelin.cmd没有任何反应
问题原因分析：
可能原因1：没有配置JAVA_HOME
解决方式1：
zeppelin.cmd第22行加入以下内容：
set JAVA_HOME=D:\Program Files\Java\jre1.8.0_111
解决方式2：配置Windows环境变量，添加JAVA_HOME环境变量。

可能原因2：Win7不支持单行过长命令，common.cmd中78行过长导致
解决方式：删除common.cmd中第74-80行的内容

## Zeppelin 如何使用

1.创建新的notebook

2.配置Interpreter，绑定spark等

3.编写spark代码，创建临时表createOrReplaceTempView，然后用 spark sql 可视化


## Zeppelin use case

https://www.zepl.com/viewer/notebooks/bm90ZTovL2lhbmRvdy8zNmNjMmU1ODJkNGQ0ZWRmYjg5MzI4MzUzYTBjNmViYi9ub3RlLmpzb24
