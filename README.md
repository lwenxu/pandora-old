mkdir -p /Users/lwen/docker/mysql/data

mkdir -p /Users/lwen/docker/mysql/conf

docker run -d --name mysql \
-p 3306:3306 \
-v /Users/lwen/docker/mysql/data:/var/lib/mysql \
-v /Users/lwen/docker/mysql/conf:/etc/mysql/conf.d \
-e MYSQL_ROOT_PASSWORD=12345678 \
mysql:5.6

配置properties数据库信息

导入 mysql 表

启动