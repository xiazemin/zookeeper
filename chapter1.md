# 环境搭建

下载地址：[http://apache.mirrors.lucidnetworks.net/zookeeper/](http://apache.mirrors.lucidnetworks.net/zookeeper/)

解压

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



