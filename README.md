## gbf proxy

该项目帮助在服务器上快速搭建gbf代理环境

考虑到系统默认仓库docker大概率太低，建议先升级

升级yum
```
sudo yum update
```
设置yum源
```
sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo
```

安装docker
```
sudo yum install docker-ce
```

安装docker-compose
```
sudo yum install docker-compose
```

启动并加入开机启动
```
sudo systemctl start docker
sudo systemctl enable docker
```



```
cd /项目目录
docker-compose up -d
```

启动后默认使用8088端口

如启动成功后代理失败，请检查防火墙是否开启且端口8088是否开放

核心代码使用 [Frizz925/gbf-proxy](https://github.com/Frizz925/gbf-proxy)
