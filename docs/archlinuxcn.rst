Arch Linux CN 镜像使用帮助
============================

镜像地址
----------

`http://mirrors.ucas.ac.cn/archlinuxcn/ <http://mirrors.ucas.ac.cn/archlinuxcn/>`_

镜像简介
----------

Arch Linux 中文社区仓库是由 Arch Linux 中文社区驱动的非官方用户仓库。

包含中文用户常用软件、工具、字体/美化包等。

使用帮助
----------

1. 在文件 ``/etc/pacman.conf`` 末尾添加

::

    [archlinuxcn]
    Server = http://mirrors.ucas.ac.cn/archlinuxcn/$arch

2. 运行 ``sudo pacman -Syy && sudo pacman -S archlinuxcn-keyring`` 以更新缓存并导入 PGP Keys

相关连接
---------

:完整的包信息列表（包名称/架构/维护者/状态）: https://github.com/archlinuxcn/repo
:官方主页: https://www.archlinuxcn.org
:仓库地址: http://repo.archlinuxcn.org
:镜像列表: https://github.com/archlinuxcn/mirrorlist-repo
