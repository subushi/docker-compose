### tomcat
### 启动服务

```
docker-compose -f docker-compose-tomcat.yml up -d 
```
> 发现 localhost+端口 访问报404错误，进入容器，把webapps删除，把webapps.dist改名为webapps即可

> 也可使用 docker cp tomcat:/usr/local/tomcat/webapps.dist ./ 将文件拷贝到本地，修改名称后删除原容器，重新启动compose文件执行数据卷映射
