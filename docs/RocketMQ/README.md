# RocketMQ

RocketMQ 是一个分布式消息中间件，前身是 MetaQ，是阿里参考 Kafka 特点研发的，开源给 Apache 基金会成为了 Apache 的顶级开源项目。


### 项目结构
- rocketmq-broker ：接受生产者发来的消息并存储（通过调用 rocketmq-store ），消费者从这里取得消息。
- rocketmq-client ：提供发送、接受消息的客户端 API。
- rocketmq-namesrv ：NameServer，类似于 Zookeeper，这里保存着消息的 Topic Name、队列等运行时的元信息。
- rocketmq-common ：通用的一些类、方法、数据结构等。
- rocketmq-remoting ：基于 Netty4 的 client/server + fastjson 序列化 + 自定义二进制协议。
- rocketmq-store ：消息、索引存储等。
- rocketmq-filtersrv ：消息过滤器 Server，需要注意的是，要实现这种过滤，需要上传代码到 MQ（一般而言，我们利用 Tag 足以满足大部分的过滤需求，如果更灵活更复杂的过滤需求，可以考虑 filtersrv 组件）。
- rocketmq-tools ：命令行工具。