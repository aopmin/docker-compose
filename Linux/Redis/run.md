# 1、使用docker-compse启动容器
```shell
docker-compose -f docker-compose-redis.yml up -d
```

# 2、关闭容器并删除容器
```shell
docker-compose -f docker-compose-redis.yml down
```

# 3、重启容器
```shell
docker-compose -f docker-compose-redis.yml restart
```