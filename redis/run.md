### redis
### 创建映射目录

```
mkdir -p /data/docker/redis/conf/
```
> 将 redis.conf 配置文件放进该目录中

### 启动服务

```
docker-compose -f docker-compose-redis.yml up -d 
```


