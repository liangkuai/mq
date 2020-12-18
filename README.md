# MQ


#### [MQ 的问题（issue#2）](https://github.com/liangkuai/mq/issues/2)
技术是把双刃剑。引入新技术能够解决很多问题，但同时也会产生不少问题。

- 如何保证消息不被重复消费？
- 如何保证顺序消费？
- 消息堆积问题

### Intro
- [x] [为什么要用 MQ？（issue#1）](https://github.com/liangkuai/mq/issues/1)
    - 异步
    - 解耦
    - 削峰
- [ ] [MQ 的问题]()
    - 如何保证顺序消费？
    - 如何解决重复消费问题？
    - 消息堆积
    - 分布式事务



- [ ] [MQ 的模型](/docs/MQ模型.md)
- [ ] [MQ 选型](/docs/MQ选型.md)


### RocketMQ
- [intro](/docs/RocketMQ/README.md)
- [ ] [架构](/docs/RocketMQ/架构.md)
    - Broker
    - NameServer
    - Producer
    - Consumer
- [ ] [RocketMQ 的消息模型](/docs/RocketMQ/RocketMQ的消息模型.md)

- [ ] [消费](/docs/RocketMQ/消费.md)
    - 回溯消费

- [问题](/docs/RocketMQ/问题.md)
    - [ ] 如何保证顺序消费？
    - [x] 如何避免重复消费？
        - 消息重复
        - 消息去重
    - [ ] 消息堆积

- [x] [事务消息](/docs/RocketMQ/事务消息.md)
    - 消息回查
    - 事务消息与分布式事务