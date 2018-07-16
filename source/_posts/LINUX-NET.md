title: Linux Net
author: Hongsen
tags:
  - linux
categories: []
date: 2018-07-16 22:50:00
---
/etc/sysconfig/network-scripts/ifcfg-eth0

设置on boot yes

设置桥接


DEVICE=eth0
HWADDR=08:00:27:A5:3B:18
TYPE=Ethernet
UUID=827cc125-e9fd-4e75-bf63-f6a20025a816
ONBOOT=yes
NM_CONTROLLED=yes
BOOTPROTO=static
IPADDR=192.168.0.113
NETMASK=255.255.255.0
GATEWAY=192.168.0.1
                                                                                               
时间同步

/usr/sbin/ntpdate pool.ntp.org

johnson.yang@tp-link.com

http://www.10fw.co.jp/index.html


IP地址不同的情况下

查看 /etc/sysconfig/network-scripts/ifcfg-eth0的MAC地址
是否和/etc/udev/rules.d/70-persistent-net.rules的地址对应