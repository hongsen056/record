title: Redis Codeignter Config
author: Hongsen
tags:
  - linux
categories: []
date: 2018-07-16 22:57:00
---

###### Codeigniter配置

* application/config/redis.php 

* $config['socket_type'] = 'tcp'; //`tcp` or `unix`
* $config['host'] = '127.0.0.1';
* $config['password'] = NULL;
* $config['port'] = 6379;
* $config['timeout'] = 0;


###### 远程连接

* /etc/redis.conf
* protected-mode no 设置为no
* #Bind 127.0.0.1 注释这行