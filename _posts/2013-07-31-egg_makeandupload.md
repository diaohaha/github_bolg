---
layout: post
title: egg的制作和上传
---

#egg文件的制作和上传#

##1.基本知识需求

>首先必须对python熟悉，编写基本程序。

>python argparse 模块的熟悉，如果你编写的是终端运行的程序的话，argparse提供了强大的终端解析功能。

>python setuptools的运行的基本理解（python 下包的管理安装机制）.其中的的setup.py文件了解

>最后就是setuptool 提供的包形成上传命令

##2.主要步骤

* 1.创建test文件夹，写setup.py文件。（主要是：包位置，包依赖项，包的相关文件）

* 2.test文件夹中继续创建test文件夹，里边写__init__.py 文件，这里就是setup时辨认的程序开始地方。（不过一般程序是写在其他的文     件里然后在这里调用）

* 3.一些相关命令：

>python setup.py bdist_egg : 生成egg包

>python setup.py install ： 安装

>python setup.py register sdist bdist_egg upload ：上传pypi

##3.一些注意事项

>setup里写好包的依赖关系，写好需要文件。

卧操，不写了。

##4.示例

参考连接[an example](https://github.com/diaohaha/passkeeper)

