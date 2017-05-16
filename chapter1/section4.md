# znode增删改查

通过运行create /zk\_test my\_data，在server1创建一个新的znode。这将创建一个新的znode节点和一个相关联的字符串"my\_data“

\[zk: 127.0.0.1:2183\(CONNECTED\) 2\]    ls /

\[zookeeper\]

\[zk: 127.0.0.1:2183\(CONNECTED\) 3\] create /zk\_test my\_data

Created /zk\_test

\[zk: 127.0.0.1:2183\(CONNECTED\) 4\] ls /

\[zookeeper, zk\_test\]

\[zk: 127.0.0.1:2183\(CONNECTED\) 5\] get /zk\_test

my\_data

cZxid = 0x200000005

ctime = Tue May 16 09:40:24 CST 2017

mZxid = 0x200000005

mtime = Tue May 16 09:40:24 CST 2017

pZxid = 0x200000005

cversion = 0

dataVersion = 0

aclVersion = 0

ephemeralOwner = 0x0

dataLength = 7

numChildren = 0

\[zk: 127.0.0.1:2183\(CONNECTED\) 6\] set /zk\_test junk

cZxid = 0x200000005

ctime = Tue May 16 09:40:24 CST 2017

mZxid = 0x200000006

mtime = Tue May 16 09:41:28 CST 2017

pZxid = 0x200000005

cversion = 0

dataVersion = 1

aclVersion = 0

ephemeralOwner = 0x0

dataLength = 4

numChildren = 0

从节点查看和删除



