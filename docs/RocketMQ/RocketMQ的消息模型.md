# RocketMQ 的消息模型


### Producer Group（生产者组）

代表某一类生成者，一般生产同一类消息。一个机器上的一个 RocketMQ Producer Client 就是一个 Producer，多个合起来就是 Group。



### Consumer Group（消费者组）

代表某一类消费者，一般消费同一类消息。一个机器上的一个 RocketMQ Consumer Client 就是一个 Consumer，多个合起来就是 Group。



### Topic（主题）

代表某一类消息。

- 主题中包含多个队列；
- 一个队列只会被一个消费者消费；
- 一般消费者组中的消费者个数和主题中的队列个数相同。