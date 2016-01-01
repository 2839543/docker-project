在本机搭建wordpress环境命令如下：

docker run -d -p 3306:3306 -e MYSQL_ROOT_PASSWORD=root --name mysql mysql:5.5 

docker run --name wordpress -e WORDPRESS_DB_HOST=192.168.33.131     -e WORDPRESS_DB_USER=root -e WORDPRESS_DB_PASSWORD=root -d -p 8889:80  wordpress


注意：写成docker-compose.yml 后就出现问题。

MySQL Connection Error: (2006) MySQL server has gone away