Arch Linux 镜像使用帮助
============================

镜像地址
----------

`http://mirrors.ucas.ac.cn/archlinux/ <http://mirrors.ucas.ac.cn/archlinux/>`_

使用帮助
----------

1. 在文件 ``/etc/pacman.d/mirrorlist`` 顶端添加

::

    Server = http://mirrors.ucas.ac.cn/archlinux/$repo/os/$arch

2. 运行 ``sudo pacman -Syy`` 以更新缓存

相关连接
---------

:官方主页:  https://www.archlinux.org/
:Wiki:  https://wiki.archlinux.org/
:镜像列表: https://www.archlinux.org/mirrors/
