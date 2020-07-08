创建或修改 /etc/docker/daemon.json 文件

# vi /etc/docker/daemon.json
{
    "registry-mirrors": ["https://registry.docker-cn.com"]
}
systemctl restart docker.service
Docker中国区官方镜像
https://registry.docker-cn.com

网易
http://hub-mirror.c.163.com

ustc 
https://docker.mirrors.ustc.edu.cn

中国科技大学
https://docker.mirrors.ustc.edu.cn

阿里云容器  服务
https://cr.console.aliyun.com/
