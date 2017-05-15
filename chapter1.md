# 环境搭建

下载地址：[http://apache.mirrors.lucidnetworks.net/zookeeper/](http://apache.mirrors.lucidnetworks.net/zookeeper/)

在主文件夹下建立一个zookeeper文件夹，在zookeeper文件夹里建立三个文件夹server1,server2,server3,

然后每个文件夹里面解压一个zookeeper的下载包，并且还建了几个文件夹，总体结构如下,最后那个是下载过来压缩包的解压文件

data,dataLog,logs,zookeeper-3.4.3

那么首先进入data目录，创建一个myid的文件，里面写入一个数字，比如我这个是server1,那么就写一个1，server2对应myid文件就写入2，server3对应myid文件就写个3

localhost:zookeeper-3.4.6 didi$ ls

CHANGES.txt            docs

LICENSE.txt            ivy.xml

NOTICE.txt            ivysettings.xml

README.txt            lib

README\_packaging.txt        recipes

bin                src

build.xml            zookeeper-3.4.6.jar

conf                zookeeper-3.4.6.jar.asc

contrib                zookeeper-3.4.6.jar.md5

dist-maven            zookeeper-3.4.6.jar.sha1

localhost:zookeeper-3.4.6 didi$ mkdir data

localhost:zookeeper-3.4.6 didi$ mkdir dataLog

localhost:zookeeper-3.4.6 didi$ mkdir logs

localhost:zookeeper-3.4.6 didi$ cd data

localhost:data didi$ echo 1 &gt; myid

localhost:data didi$ cat myid

1

在配置文件末尾加：



在文件末尾添加如下内容：

server.1=127.0.0.1:2888:3888

server.2=127.0.0.1:2889:3889

server.3=127.0.0.1:2890:3890

