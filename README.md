## Zeppelin

# Zeppelin mac 安装步骤：
1.官网下载二进制文件进行安装，zeppelin-0.8.1-bin-all.tgz, 
下载链接https://zeppelin.apache.org/download.html

为了保证系统正常启动，确保的 zeppelin.server.port 属性的端口不被占用，默认是8080。

2.解压，进入Zeppelin 安装目录的bin文件夹下，使用以下命令启动进程：

./zeppelin-daemon.sh start

若需要停止，可以使用以下命令停止进程：

./zeppelin-daemon.sh stop

3.Check out the Zeppelin web notebook at http://localhost:8080

# Zeppelin 如何使用

1.创建新的notebook

2.配置Interpreter，绑定spark等

3.编写spark代码，创建临时表createOrReplaceTempView，然后用 spark sql 可视化

