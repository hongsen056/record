title: Mysql Privileges
author: Hongsen
tags:
  - linux
categories: []
date: 2018-07-16 22:52:00
---


* GRANT ALL PRIVILEGES ON *.* TO 'root'@'192.168.0.55' IDENTIFIED BY '123456' WITH GRANT OPTION;

* GRANT ALL PRIVILEGES ON *.* TO 'root'@'192.168.0.190' IDENTIFIED BY '' WITH GRANT OPTION;

* GRANT ALL PRIVILEGES ON *.* TO 'root'@'%' IDENTIFIED BY '' WITH GRANT OPTION;

* grant all privileges on *.* to sh@'%' identified by ''; 

* select host,user,password from user;

* FLUSH PRIVILEGES;


 
###### 忘记密码的时候

* systemctl stop mysqld

###### 跳过系统权限
* vi /etc/my.cnf
* skip-grant-tables

* systemctl start mysqld

* use mysql
* UPDATE user SET * authentication_string=password('123456') WHERE user='root';
* flush privileges;

* /etc/my.cnf 
* skip-grant-tables  # 削除


###### 查看密码设置

* SHOW VARIABLES LIKE 'validate_password%';

###### 修改到低权限
* SET GLOBAL validate_password_length=4;
* SET GLOBAL validate_password_policy=LOW;
