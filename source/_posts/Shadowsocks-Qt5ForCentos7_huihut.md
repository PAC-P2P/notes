---

title: Shadowsocks-Qt5 For Centos 7
date: 2017-03-25 10:41:40
tags:
	- Shadowsocks
	- Linux
categories: 
	- Notes
	
---

Shadowsocks-Qt5 installation and Proxy in Centos 7

<!-- more -->

## Install
 
If you use the traditional `yum` package management tool, 

you need to download the appropriate version of the `repo` file from the [Copr](https://copr.fedorainfracloud.org/coprs/librehat/shadowsocks/) to `/etc/yum.repos.d/`, 

and then install through `yum`.

As follows:



    # Centos 7
    wget https://copr.fedorainfracloud.org/coprs/librehat/shadowsocks/repo/epel-7/librehat-shadowsocks-epel-7.repo
    
    sudo mv librehat-shadowsocks-epel-7.repo /etc/yum.repos.d/
 
    sudo yum update
    sudo yum install -y shadowsocks-qt5
    
<!-- more -->

    
## Config
 Explanation of the fields:

Name|	Explanation
---|---
server |	the address your server listens
server_port|	server port
local_address|	the address your local listens
local_port| local port
password |	password used for encryption
timeout |	in seconds
method	| default: “aes-256-cfb”, see Encryption
fast_open |	use TCP_FASTOPEN, true / false
workers |	number of workers, available on Unix/Linux

## Proxy

Go to `Settings`-`Network`-`Network proxy`, **turn on proxy**.

Use the `sock` proxy

local_address:	the address your local listens (default:`1080`)

local_port:	local portocal (default:`127.0.0.1`)

Have fun!