### 替换 Centos 系统 Python
* ⚠️不要删除系统 `Python 2.6`，包管理工具 `yum` 是用 Python 2.6 写的，删了 yum 就废了。
  * 如果系统 yum/python 炸了，拯救方案看这里：[CentOS7修复python拯救yum](https://cloud.tencent.com/developer/article/1567524)
* 替换步骤：
  * 官网下载需要版本的安装包
  * 解压进入代码根目录
  * 一行搞定，需要 root 权限，`./configure --enable-shared && sudo make altinstall`
