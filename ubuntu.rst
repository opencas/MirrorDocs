Ubuntu 镜像使用帮助
============================

镜像地址
----------

`http://mirrors.opencas.org/ubuntu/ <http://mirrors.opencas.org/ubuntu/>`_

使用帮助
----------

1. 编辑 ``/etc/apt/source.list``,以ubuntu16.04为例,其他发行版改相应代号

::
	
		deb http://mirrors.opencas.org/ubuntu/ xenial main restricted #deb http://mirrors6.tuna.tsinghua.edu.cn/ubuntu/ xenial-updates main restricted
		deb http://mirrors.opencas.org/ubuntu/ xenial universe
		deb http://mirrors.opencas.org/ubuntu/ xenial-updates universe
		deb http://mirrors.opencas.org/ubuntu/ xenial multiverse
		deb http://mirrors.opencas.org/ubuntu/ xenial-updates multiverse
		deb http://mirrors.opencas.org/ubuntu/ xenial-backports main restricted universe multiverse
		deb http://mirrors.opencas.org/ubuntu/ xenial-security main restricted
		deb http://mirrors.opencas.org/ubuntu/ xenial-security universe
		deb http://mirrors.opencas.org/ubuntu/ xenial-security multiverse
	

2. 运行 ``sudo apt update`` 以更新缓存

相关连接
---------

:官方主页:  https://www.ubuntu.com/
:Wiki:  https://wiki.ubunut.com/
:镜像列表: http://cn.archive.ubuntu.com/ubuntu/
