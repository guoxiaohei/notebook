```
yum update

安装erlang
yum install epel-release
yum install erlang

安装rabbitmq-server
yum install rabbitmq-server

启动
/usr/lib/rabbitmq/bin/rabbitmq-server -detached

日志文件：
/var/log/rabbitmq/rabbit@localhost.log

配置文件
/etc/rabbitmq/rabbitmq.config

修改guest可以远程访问：
%% {loopback_users, []},
改为：
{loopback_users, []}

启用web控制台：
/usr/lib/rabbitmq/bin/rabbitmq-plugins enable rabbitmq_management
重启rabbitmq

列出所有的队列
/usr/lib/rabbitmq/bin/rabbitmqctl list_queues

删除所有的队列
/usr/lib/rabbitmq/bin/rabbitmqctl reset
/usr/lib/rabbitmq/bin/rabbitmqctl stop_app
/usr/lib/rabbitmq/bin/rabbitmqctl start_app
```

