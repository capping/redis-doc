# Documentation

注意：Redis文档也可以在[Redis-doc github存储库](https://github.com/antirez/redis-doc)中以原始格式(计算机友好)获得。Redis文档是在[知识共享署名- sharealike 4.0国际许可](https://creativecommons.org/licenses/by-sa/4.0/)
下发布的。

## Programming with Redis(程序设计与Redis)
- Redis实现的命令的完整列表(The full list of commands)，以及他们各自的详细文档
- Pipelining:学习如何同时发送多个命令，节省往返时间
- Redis Pub/Sub:Redis是一个快速的、稳定的发布/订阅消息系统！看过来
- Redis Lua scripting:Redis Lua脚本功能文档
- Debugging Lua scripts:Redis 3.2 为Redis引入了一个本地的Lua调试器
- Memory optimization:了解Redis如何使用RAM，并学习一些技巧来减少内存的使用
- Expires:Redis允许为每个key设置不同的生存时间，以便秘钥过期时自动从服务器删除
- Redis as a LRU cache:如何配置和使用Redis作为缓存与固定数量的内存和自动回收key
- Redis transactions:可以将命令组合在一起，以便将他们作为单个事务执行
- Mass insertion data:如何在短时间内向Redis实例添加大量预先存在或生成的数据
- Partitioning:如何在多个Redis实例之间分发数据
- Distributed locks:使用Redis实现分布式锁管理器
- Redis keyspace notifications: Get notifications of keyspace events via Pub/Sub (Redis 2.8 or greater)
- Creating secondary indexes with Redis:使用Redis数据结构创建辅助索引、组合索引和遍历图

