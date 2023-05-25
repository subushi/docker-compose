### gitlab
### 启动服务

```
docker-compose -f docker-compose-gitlab.yml up -d 
```

> 登录服务 localhost:9980 默认登录账号为root
> 某些 gitlab 版本启动后自带初始化密码，使用以下命令进行查看

```
docker exec -it gitlab grep 'Password:' /etc/gitlab/initial_root_password
```

> 首次启动后在映射目录 /data/docker/gitlab/etc 下的 gitlab.rb 中添加以下内容

```
external_url 'http://110.40.196.124:9980'               http克隆链接
gitlab_rails['gitlab_ssh_host'] = '110.40.196.124'      ssh克隆链接
gitlab_rails['gitlab_shell_ssh_port'] = 9922            ssh克隆端口
```

> 添加成功后删除原容器，打开yml文件中注释的端口再次启动即可

```
- "9980:9980"
- "9922:9922"
- "9443:9443"
```
