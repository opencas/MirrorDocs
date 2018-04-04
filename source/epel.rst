EPEL 镜像使用帮助
======================

镜像地址
----------

`http://mirrors.ucas.ac.cn/epel/ <http://mirrors.ucas.ac.cn/epel/>`_

使用帮助
----------

1. 首先安装 ``epel-release``

::

    yum install epel-release

2. 备份文件 ``/etc/yum.repos.d/epel.repo``

::

  mv /etc/yum.repos.d/epel.repo /etc/yum.repos.d/epel.repo.backup

3. 根据系统版本，将相对应的内容写入 ``epel.repo`` 中

**CentOS 5:**

::

    [epel]
    name=Extra Packages for Enterprise Linux 5 - $basearch
    baseurl=http://mirrors.ucas.ac.cn/epel/5/$basearch
    #mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=epel-5&arch=$basearch
    failovermethod=priority
    enabled=1
    gpgcheck=1
    gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-5

    [epel-debuginfo]
    name=Extra Packages for Enterprise Linux 5 - $basearch - Debug
    baseurl=http://mirrors.ucas.ac.cn/epel/5/$basearch/debug
    #mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=epel-debug-5&arch=$basearch
    failovermethod=priority
    enabled=0
    gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-5
    gpgcheck=1

    [epel-source]
    name=Extra Packages for Enterprise Linux 5 - $basearch - Source
    baseurl=http://mirrors.ucas.ac.cn/epel/5/SRPMS
    #mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=epel-source-5&arch=$basearch
    failovermethod=priority
    enabled=0
    gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-5
    gpgcheck=1

**CentOS 6:**

::

    [epel]
    name=Extra Packages for Enterprise Linux 6 - $basearch
    baseurl=http://mirrors.ucas.ac.cn/epel/6/$basearch
    #mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=epel-6&arch=$basearch
    failovermethod=priority
    enabled=1
    gpgcheck=1
    gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-6

    [epel-debuginfo]
    name=Extra Packages for Enterprise Linux 6 - $basearch - Debug
    baseurl=http://mirrors.ucas.ac.cn/epel/6/$basearch/debug
    #mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=epel-debug-6&arch=$basearch
    failovermethod=priority
    enabled=0
    gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-6
    gpgcheck=1

    [epel-source]
    name=Extra Packages for Enterprise Linux 6 - $basearch - Source
    baseurl=http://mirrors.ucas.ac.cn/epel/6/SRPMS
    #mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=epel-source-6&arch=$basearch
    failovermethod=priority
    enabled=0
    gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-6
    gpgcheck=1

**CentOS 7:**

::

    [epel]
    name=Extra Packages for Enterprise Linux 7 - $basearch
    baseurl=http://mirrors.ucas.ac.cn/epel/7/$basearch
    #mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=epel-7&arch=$basearch
    failovermethod=priority
    enabled=1
    gpgcheck=1
    gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-7

    [epel-debuginfo]
    name=Extra Packages for Enterprise Linux 7 - $basearch - Debug
    baseurl=http://mirrors.ucas.ac.cn/epel/7/$basearch/debug
    #mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=epel-debug-7&arch=$basearch
    failovermethod=priority
    enabled=0
    gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-7
    gpgcheck=1

    [epel-source]
    name=Extra Packages for Enterprise Linux 7 - $basearch - Source
    baseurl=http://mirrors.ucas.ac.cn/epel/7/SRPMS
    #mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=epel-source-7&arch=$basearch
    failovermethod=priority
    enabled=0
    gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-7
    gpgcheck=1


4. 运行 ``sudo yum makecache`` 以更新缓存

相关连接
---------

:官方主页: https://fedoraproject.org/wiki/EPEL
:Wiki: https://admin.fedoraproject.org/mirrormanager/mirrors
:镜像列表: https://www.centos.org/download/mirrors/
