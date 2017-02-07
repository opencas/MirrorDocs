OpenCAS MirrorDocs
=======

## Syncing Mirrors

Apache ArchLinux Centos CRAN CTAN Cygwin Deepin Deepin-cd Eclipse EPEL Gentoo Gentoo-Portage GNU Mariadb Pypi Raspbian Ubuntu Ubuntu-Release Ubuntu-Cloud

## Tools & Language

Sphinx with reStructuredText.

## Contribute

0\. Fork

1\. Choose one mirror in the `todo` list in `index.rst`

2\. Write the help file. Notice that the filename must be `MIRRORNAME.rst`.

3\. The help file should include 3 parts:

`镜像地址`，`使用帮助` 及 `相关链接`

You can follow the `centos.rst`.

The mirror URL is: `http://mirrors.opencas.org/MIRRORNAME/`

4\. Move the mirror out of the `todo` list in `index.rst`.

5\. Pull Request

## Local Test

1\. Install Python 3 & Pip

2\. Install requirements

```
$ pip3 install -r requirements.txt
```

3\. Build & Test

```
$ make html
$ open ./build/html/index.html
```

