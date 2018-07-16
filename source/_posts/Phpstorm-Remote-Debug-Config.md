title: Phpstorm Remote Debug Config
author: Hongsen
tags:
  - linux
categories: []
date: 2018-07-16 23:03:00
---
###### Debug Config



* zend_extension="/opt/remi/php70/root/usr/lib64/php/modul* es/xdebug.so"
* xdebug.remote_enable=1
* xdebug.remote_autostart=1
* xdebug.remote_host=192.168.0.2 本地的IP
* xdebug.remote_port=9000
* xdebug.remote_log=/tmp/xdebug.log
* xdebug.idekey = "phpstorm"



                                             

###### 全部IP的debug
* zend_extension="/opt/remi/php70/root/usr/lib64/php/modul es/xdebug.so"
* xdebug.remote_enable=1
* xdebug.remote_port=9000
* xdebug.idekey = "phpstorm"
* xdebug.ide_key = "phpstorm"
* xdebug.remote_connect_back=1
* xdebug.remote_autostart=1
* xdebug.remote_handler=dbgp
* xdebug.remote_log="/var/log/xdebug.log"


* /etc/php.d/xdebug.ini