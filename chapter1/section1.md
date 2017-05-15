# 启动

$ pwd

/Users/didi/zookeeper/server1/zookeeper-3.4.6/bin

localhost:bin didi$ ./zkServer.sh start

JMX enabled by default

Using config: /Users/didi/zookeeper/server1/zookeeper-3.4.6/bin/../conf/zoo.cfg

Starting zookeeper ... STARTED

localhost:bin didi$ ./zkServer.sh status

JMX enabled by default

Using config: /Users/didi/zookeeper/server1/zookeeper-3.4.6/bin/../conf/zoo.cfg

Error contacting service. It is probably not running.

localhost:bin didi$ cd ../../../server1/zookeeper-3.4.6/b

bin/       build.xml

localhost:bin didi$ cd ../../../server2/zookeeper-3.4.6/bin

localhost:bin didi$ ls

README.txt	zkCli.cmd	zkEnv.cmd	zkServer.cmd	zookeeper.out

zkCleanup.sh	zkCli.sh	zkEnv.sh	zkServer.sh

localhost:bin didi$ ./zkServer.sh start

JMX enabled by default

Using config: /Users/didi/zookeeper/server2/zookeeper-3.4.6/bin/../conf/zoo.cfg

Starting zookeeper ... STARTED

localhost:bin didi$ ./zkServer.sh status

JMX enabled by default

Using config: /Users/didi/zookeeper/server2/zookeeper-3.4.6/bin/../conf/zoo.cfg

Mode: leader

localhost:bin didi$ cd ../../../server3/zookeeper-3.4.6/bin

localhost:bin didi$ ./zkServer.sh start

JMX enabled by default

Using config: /Users/didi/zookeeper/server3/zookeeper-3.4.6/bin/../conf/zoo.cfg

Starting zookeeper ... STARTED

localhost:bin didi$ ./zkServer.sh status

JMX enabled by default

Using config: /Users/didi/zookeeper/server3/zookeeper-3.4.6/bin/../conf/zoo.cfg

Mode: follower

