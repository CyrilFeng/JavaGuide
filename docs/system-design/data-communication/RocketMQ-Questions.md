生产者发送事务消息，假设该事务消息 Topic 为 Topic1-Trans，Broker 得到后首先更改该消息的 Topic 为 Topic1-Prepared，该 Topic1-Prepared 对消费者不可见。然后定时回调生产者的本地事务A执行状态，根据本地事务A执行状态，来是否将该消息修改为 Topic1-Commit 或 Topic1-Rollback，消费者就可以正常找到该事务消息或者不执行等

>注意，就算是事务消息最后回滚了也不会物理删除，只会逻辑删除该消息

 

### 2.1.9 广播消费与集群消费

1. 消息消费区别：广播消费，订阅该 Topic 的消息者们都会消费**每个**消息。集群消费，订阅该 Topic 的消息者们只会有一个去消费**某个**消息
2. 消息落盘区别：具体表现在消息消费进度的保存上。广播消费，由于每个消费者都独立的去消费每个消息，因此每个消费者各自保存自己的消息消费进度。而集群消费下，订阅了某个 Topic，而旗下又有多个 MessageQueue，每个消费者都可能会去消费不同的 MessageQueue，因此总体的消费进度保存在 Broker 上集中的管理

### 2.1.10 RocketMQ 不使用 ZooKeeper 作为注册中心的原因，以及自制的 NameServer 优缺点？

1. ZooKeeper 作为支持顺序一致性的中间件，在某些情况下，它为了满足一致性，会丢失一定时间内的可用性，RocketMQ 需要注册中心只是为了发现组件地址，在某些情况下，RocketMQ 的注册中心可以出现数据不一致性，这同时也是 NameServer 的缺点，因为 NameServer 集群间互不通信，它们之间的注册信息可能会不一致
2. 另外，当有新的服务器加入时，NameServer 并不会立马通知到 Produer，而是由 Produer 定时去请求 NameServer 获取最新的 Broker/Consumer 信息（这种情况是通过 Producer 发送消息时，负载均衡解决）
 
 
 
