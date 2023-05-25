### nginx
### 创建映射目录

```
mkdir -p /data/docker/nginx/conf/
```
> 将 nginx.conf 配置文件放进该目录中

### 启动服务

```
docker-compose -f docker-compose-nginx.yml up -d 
```

