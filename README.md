# 实验一： DOL环境开发配置

## Description

The distributed operation layer (DOL) is a software development framework to program parallel applications. The DOL allows to specify applications based on the Kahn process network model of computation and features a simulation engine based on systemC. Moreover, the DOL provides an XML-based specification format to describe the implementation of a parallel application on a multi-processor systems, including binding and mapping.

##How to install

#### 1.安装必要环境
    	$ sudo apt-get update
   	$ sudo apt-get install ant
   	$ sudo apt-get install openjdk-7-jdk
    	$ sudo apt-get install unzip

#### 2.下载文件到虚拟机

*方法一：从主机复制到虚拟机。
*方法二：在虚拟机上下载
	$ sudo wget http://www.accellera.org/images/downloads/standards/systemc/systemc-2.3.1.tgz
	$ sudo wget http://www.tik.ee.ethz.ch/~shapes/downloads/dol_ethz.zip
#### 3.解压文件

*新建dol文件夹
$ mkdir dol

*将dolethz.zip解压到 dol文件夹中
$ unzip dol_ethz.zip -d dol

*解压systemc
$ tar -zxvf systemc-2.3.1.tgz

#### 4.编译systemc

*解压后进入systemc-2.3.1的目录下
$ cd systemc-2.3.1

*新建一个临时文件夹objdir
$ mkdir objdir

*进入该文件夹objdir
$ cd objdir

*运行configure (能根据系统的环境设置一下参数，用于编译)
$ ../configure CXX=g++ --disable-async-updates

Experimental experience

Github可以进行版本控制，也可以共享，有利于团队内共享代码，完成任务。按照步骤一步一步安装DOL环境，在不断网的情况下就可以顺利配置成功。
Workdown的排版好看，简易，比word好控制。
