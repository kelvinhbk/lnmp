# lnmp
php环境

# 安装docker-compose
需要在运行docker容器的主机上安装docker-compose，可以参照官方文档手动安装，也可以使用ezhttp的一键安装工具(推荐)安装。如：

```
wget centos.bz/ezhttp.zip
unzip ezhttp.zip
cd ezhttp-master
./start.sh
```
之后会弹出一个菜单，输入2选择Some Useful Tools,然后输入18选择安装docker和compose。


# 编写Dockerfile
clone以上在阿里云Kelude创建的Dockerfile镜像到本地，在此项目中创建centos.bz,然后在centos.bz目录分别创建mysql,nginx,php目录，用于存放它们各自Dockerfile及配置文件。
这里我们还约定以下目录：

* /home/docker/nginx/logs/centos.bz：存放www.centos.bz网站的日志
* /home/docker/nginx/www/centos.bz: 存放www.centos.bz网站的文件
* /home/docker/php: 存放php-fpm的日志
* /home/docker/mysql：mysql data目录

