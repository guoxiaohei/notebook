### 1.TPS: Transactions Per Second（每秒传输的事物处理个数）

Transactions Per Second（每秒传输的事物处理个数，即服务器每秒处理的事务数。）

1）用户请求服务器

2）服务器自己的内部处理

3）服务器返回给用户

这三个过程，每秒能够完成N个这三个过程，Tps也就是N；（业务TPS = CAPS × 每个呼叫平均TPS）

TPS是软件测试结果的测量单位。一个事务是指一个客户机向服务器发送请求然后服务器做出反应的过程。客户机在发送请求时开始计时，收到服务器响应后结束计时，以此来计算使用的时间和完成的事务个数。

一般的，评价系统性能均以每秒钟完成的技术交易的数量来衡量。系统整体处理能力取决于处理能力最低模块的TPS值。

### 2.QPS: Queries Per Second(每秒查询率)

Queries Per Second意思是“每秒查询率”，是一台服务器每秒能够相应的查询次数，是对一个特定的查询服务器在规定时间内所处理流量多少的衡量标准。

Qps基本类似于Tps，但是不同的是，对于一个页面的一次访问，形成一个Tps；但一次页面请求，可能产生多次对服务器的请求，服务器对这些请求，就可计入“Qps”之中。