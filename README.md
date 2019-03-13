# Introduction to Redis (介绍Redis)

[Documentation](./Documentation.md)

Redis是一个开源的(BSD许可)，内存中的数据结构存储系统，它可以用作数据库，缓存和消息中间件。它支持多种类型的数据结构，如[strings](./strings.md)，hashes，lists，sets，有范围查询功能的 sorted sets，bitmaps，
hyperloglogs，地理空间(geospatial)的索引半径查询和流。Redis内置了复制(replication)，Lua脚本，LRU回收(LRU eviction)，事务(transactions) 和 不同级别的磁盘持久化(persistence),并通过Redis哨兵
(Redis Sentinel)和拥有Redis集群(Redis Cluster)的自动分区提供了高可用性(high availability)。

你可以在这些类型上运行原子操作，例如追加字符串(appending to a string)；在hash中自增值(incrementing the value in a hash)；向对列中压如一个元素(pushing an element to a list)；计算set交集
(computing set intersection)，并集(union)和差集(difference);或者在sorted set中获取最高排名的成员。

为了实现它的出色的性能，Redis使用内存中的数据集。基于你的使用场景，你有两种持久化的方法，一个是每隔一段时间将数据转存到磁盘，另一种是将每个命令追加到日志中。持久化可以选择性的关闭，如果你只需要一个功能丰富的、联网的
内存缓存。

Redis通过简单的配置就支持主备异步复制，具有非常快速的非阻塞首次同步，在网路断线时自动重新连接和部分重新同步。

另外的功能包括：
- 事务 (Transactions)
- 发布/订阅 (Pub/Sub)
- Lua脚本 (Lua scripting)
- 设置过期时间 (Keys with a limited time-to-live)
- LRU淘汰机制 (LRU eviction of keys)
- 自动故障切换 (Automatic failover)

你可以在大多数编程语言中都可以使用Redis。

Redis使用`ANSI C`编写，可以在大多数可移植系统(POSIX systems)中工作，例如Linux，*BSD，OS X，不需要外部依赖。Linux和OS X是开发和测试Redis的两个操作系
统，我们建议使用Linux进行部署。Redis可以在像SmartOS这样的solaris派生系统中工作，但是支持是最好的。目前还没有官方对Windows构建的支持，但微软开发并维护了
Win-64的Redis端口。
