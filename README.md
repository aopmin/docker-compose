##  一、环境准备

---

### 1. Linux上docker-compose环境准备

1、将`docker-compose/Linux/env`目录下的docker-compose文件复制到本机`/usr/local/bin`目录下;

```shell
cp docker-compose  /usr/local/bin

cd /usr/local/bin
```

2、为docker-compose文件添加可执行权限
```shell
chmod +x /usr/local/bin/docker-compose
```

3、查看版本信息
```shell
docker-compose -version
```
4、 重启docker服务:

```shell
systemctl restart docker.service
```

