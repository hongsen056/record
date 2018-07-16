title: SELinux Close
author: Hongsen
date: 2018-07-16 22:39:06
tags: [linux]
---
###### 查看SELinux：
* /usr/sbin/sestatus -v      
* 如果SELinux status参数为enabled即为开启状态
* SELinux status:                 enabled
* getenforce       

###### 关闭SELinux：
* 临时关闭（不用重启机器）：
setenforce 0   设置SELinux 成为permissive模式
             setenforce 1 设置SELinux 成为enforcing模式
* 修改配置文件需要重启机器：
修改/etc/selinux/config 文件
将SELINUX=enforcing改为SELINUX=disabled
重启机器即可


http://wiki.workerman.net/Error3