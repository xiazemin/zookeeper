# BOOKKEEPER

Apache的项目ZooKeeper有了一个兄弟项目: BookKeeper。



BookKeeper是一个可靠地记录日志流的一个系统， 它是被设计来记录Write Ahead Log的（操作具体数据结构之前先记录日志），Write Ahead Log在数据库里面很常见， 实际上BookKeeper的创意来自于hadoop里面的NameNode，NameNode在把数据写入内存之前先写入磁盘日志，但是写入本地磁盘有个问题：如果这台机器的磁盘坏了， 那么数据还是恢复不了。BookKeeper就是为了弥补这个缺陷的，这样之后NameNode不用写入自己的本地磁盘，而是写入BookKeeper系统，而可靠性则由BookKeeper来保证。虽然BookKeeper是为hadoop设计的，但是对于任何需要这种可靠性的日志的系统并且系统里面只有个线程写日志的话，那么都可以用这个系统。



BookKeeper里面的服务器叫做: bookies， 日志流叫做ledgers, BookKeeper被设计成高可靠性的， 即使有写bookie挂掉了，只要有足够数量的bookie还在正常工作的话，那么整个BookKeeper集群就可以正常工作。



跟大多数可靠性系统一样，BookKeeper为把同一份数据存多份在各个bookie上面。



BookKeeper的数据模型是一个扁平的结构，每个ledger由一个long型的key唯一确定。ledgers只支持append操作，而且同时只能有一个单线程来写。

项目主页：http://www.open-open.com/lib/view/home/1323312523671

