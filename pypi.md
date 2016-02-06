# pypi镜像使用帮助
## 临时使用
`pip install -i https://pypi.mirrors.opencas.cn/simple package-name`

注: **simple** 不能少, 是 **https** 而不是 http

## 默认使用
修改 `~/.pip/pip.conf` (没有就创建一个)， 修改 `index-url`

`index-url = https://pypi.mirrors.opencas.cn/simple`

