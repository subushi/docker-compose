### alertmanager-邮件报警
### 创建映射目录

```
mkdir -p /data/docker/alertmanager
```
> 将 alertmanager.yml 配置文件放进该目录中

### 启动服务

```
docker-compose -f docker-compose-alertmanager.yml up -d 
```

> 登录服务 localhost:9093
