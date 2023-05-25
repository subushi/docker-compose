### mysql
### 创建映射目录

```
mkdir -p /data/docker/mysql/conf/
```
> 将 my.cnf 配置文件放进该目录中

### 启动服务

```
docker-compose -f docker-compose-mysql.yml up -d
```

