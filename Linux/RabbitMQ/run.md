## 一、RabbitMQ单机版

---

```shell

# 为当前目录下的rabbitmq目录赋予权限(读、写、执行)
mkdir rabbitmq/
chmod -R 777 ./rabbitmq
# 运行 [ 注：如果之前有安装过，需要删除rabbitmq相关的存储数据(如:rabbitmq容器映射到宿主机目录)，再重装，否则会出现一定问题！ ]
# docker-compose -f docker-compose-rabbitmq-3.8-management.yml -p rabbitmq up -d

# 运行 rabbitmq-3.8-management版本镜像容器(带-d表示后台启动,不带-d表示前台启动)
 docker-compose -f docker-compose-rabbitmq.yml up -d

# 进入容器
docker exec -it rabbitmq /bin/bash

# 开启管理界面 
rabbitmq-plugins enable rabbitmq_management

# 开启延时插件
rabbitmq-plugins enable rabbitmq_delayed_message_exchange

# 查看已安装插件
rabbitmq-plugins list
```
>测试
> 
web管理端：ip地址:15672 ,登录账号密码：admin/123456