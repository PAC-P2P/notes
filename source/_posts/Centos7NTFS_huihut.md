---

title: Centos 7 挂载 NTFS 分区
date: 2017-03-25 11:03:29
tags:
	- Linux
categories: 
	- Notes
	
---

Centos 7 挂载 NTFS 分区

<!-- more -->


## NTFS-3G

使用 NTFS-3G 实现，可以挂载 NTFS，还可以挂载 HFS+ 等，以下是在 Centos 7 下安装 NTFS-3G 及挂载 NTFS 分区

    wget -O /etc/yum.repos.d/epel.repo http://mirrors.aliyun.com/repo/epel-7.repo
    
    sudo yum update
    
    sudo yum install ntfs-3g
