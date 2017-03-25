---

title: Centos 7 设置开机自动联网
date: 2017-03-25 10:59:48
tags:
	- Linux
categories: 
	- Notes
	
---

Centos 7 设置开机自动联网


<!-- more -->



    ls /etc/sysconfig/network-scripts/
    
    # 找到ifcfg-e`npxxx`，如我的是`rk-scripts`
    
    sudo vim /etc/sysconfig/network-scripts/ifcfg-enp4s0
   
    # 一般文件里面有下面这些 
    TYPE=Ethernet
    BOOTPROTO=dhcp
    DEFROUTE=yes
    PEERDNS=yes
    PEERROUTES=yes
    IPV4_FAILURE_FATAL=no
    IPV6INIT=yes
    IPV6_AUTOCONF=yes
    IPV6_DEFROUTE=yes
    IPV6_PEERDNS=yes
    IPV6_PEERROUTES=yes
    IPV6_FAILURE_FATAL=no
    NAME=enp4s0
    UUID=4d0c8a3a-50bf-497a-9b04-f5fba085ef08
    DEVICE=enp4s0
    ONBOOT=no
    
    # 把`ONBOOT=no`该为`  ONBOOT=yes`，保存即可。