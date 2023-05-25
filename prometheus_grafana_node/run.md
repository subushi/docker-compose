### prometheus_grafana_node
### 创建映射目录

```
mkdir -p /data/docker/prometheus/
```
> 将 prometheus.yml 配置文件放进该目录中

### 启动服务

```
docker-compose -f docker-compose-prometheus_grafana_node.yml up -d 
```
