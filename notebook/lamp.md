# lamp

## ubuntu

- sudo passwd root，可以修改root用户的密码
- su，切换到root用户
- sudo apt-get update，更新软件源

## apache2

- 安装，sudo apt-get install apache2
- sudo apache2 -v，查看版本
- ip addr，查看ip
- 在浏览器输入ip，可以看到apache2启动，网页显示“It's works!”

## php

- 安装，sudo apt-get install php7.0
- sudo php7.2 -v，查看版本
- apt-cache search libapache2-mod-php，php和apache2都装好了，需要让apache2能够识别解析php文件，我们先搜一下有没有适合php7的插件。
- sudo apt-get install libapache2-mod-php7.2，安装
- cat /etc/apache2/mods-enabled/php7.2.load，查看apache2调用的php解析文件

## mysql

- sudo apt-get install mysql-server mysql-client
- sudo apt-get install php7.2-mysql
- sudo service mysql restart，重启
- sudo tasksel install lamp-server，套装安装，一步到位。

