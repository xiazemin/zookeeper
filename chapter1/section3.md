# 使用教程

[http://blog.csdn.net/pdw2009/article/details/47324053](http://blog.csdn.net/pdw2009/article/details/47324053)

[http://zookeeper.majunwei.com/document/3.4.6/GettingStarted.html](http://zookeeper.majunwei.com/document/3.4.6/GettingStarted.html)

http://www.w3cschool.cn/zookeeper/

\[zk: 127.0.0.1:2183\(CONNECTED\) 1\] help

ZooKeeper -server host:port cmd args

```
connect host:port

get path \[watch\]

ls path \[watch\]

set path data \[version\]

rmr path

delquota \[-n\|-b\] path

quit

printwatches on\|off

create \[-s\] \[-e\] path data acl

stat path \[watch\]

close

ls2 path \[watch\]

history

listquota path

setAcl path acl

getAcl path

sync path

redo cmdno

addauth scheme auth

delete path \[version\]

setquota -n\|-b val path
```



