### nacos
### 创建映射目录

```
mkdir -p /data/docker/nacos/init.d/
```
> 将 application.properties 配置文件放进该目录中

### 启动服务

```
docker-compose -f docker-compose-nacos.yml up -d
```
> 登录服务 localhost:8848/nacos 初始默认账号密码为nacos

> 如果配置文件中读取的数据库已经存在创建好的账号和密码则使用已有的账号和密码

