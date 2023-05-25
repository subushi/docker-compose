### prometheus——普罗米修斯监控
### 创建映射目录

```
mkdir -p /data/docker/prometheus/
```
> 将 prometheus.yml 配置文件放进该目录中

### 启动服务

```
docker-compose -f docker-compose-prometheus.yml up -d 
```

> 登录服务 localhost:9090 
