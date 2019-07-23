---
layout: post
title: Flarum安装流程（附简体中文）
---

更新源  
~~~shell
sudo apt-get update
sudo apt-get upgrade
~~~
安装 apache2、openssl、mysql
~~~shell
sudo apt install apache2 openssl mysql-client mysql-server
~~~
apache2 开启重写模块
~~~shell
sudo a2enmod rewrite
sudo service apache2 restart
~~~
安装 php7.3  
~~~shell
sudo add-apt-repository ppa:ondrej/php
sudo apt-get update
sudo apt install php7.3 php7.3-mysql php7.3-curl php7.3-gd php7.3-mbstring php7.3-xml
~~~
  
安装 composer  
~~~shell
php -r "copy('https://install.phpcomposer.com/installer', 'composer-setup.php');"
php composer-setup.php
php -r "unlink('composer-setup.php');"
sudo mv composer.phar /usr/local/bin/composer
~~~
  
使用中国镜像
~~~shell
composer config -g repo.packagist composer https://packagist.phpcomposer.com
~~~
  
安装 Flarum
~~~shell
mkdir flarum
cd flarum
composer create-project flarum/flarum . --stability=beta
~~~
这里要等很久  
  
安装简体中文扩展
~~~shell
composer require csineneo/lang-simplified-chinese
~~~