Elasticsearch把操作封装为HTTP的API
1. 倒排索引
2. es索引
    1. 存放数据的地方，可以理解为mysql中的一个**数据库**
    
3. 类型
    1. 用来定义数据结构，可以理解为mysql中的**一张表**。
4. 文档
    1. 最终数据，可以理解为一个文档就是**一个记录**。
    
5. keyword类型 直接建立反向索引；text类型 先分词后建立反向索引。
- - -
分布式原理https://zhuanlan.zhihu.com/p/62892586
1. 会对数据进行切分，每个分片保存多个副本，保证分布式环境下高可用。
2. master-slaver架构，master负责集群状态信息的改变，并同步给其他节点。