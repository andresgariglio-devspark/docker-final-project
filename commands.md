docker run 
--name web 
--link mysql:mysql
-d 
-p 8081:80 
php-link:1.0


docker run
--name mysql
-v /home/ubuntu/data:/var/lib/mysql
-e MYSQL_ROOT_PASSWORD=secret
-e MYSQL_DATABASE=homestead
-e MYSQL_USER=homestead
-e MYSQL_PASSWORD=secret
-d
mysql:latest

