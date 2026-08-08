# Linux File Permission Lab

## 实验介绍

这是我的第5个网络安全基础实验。

This is my fifth cybersecurity foundation lab.

本实验主要学习 Linux 文件权限管理。


## 实验环境

System:

Kali Linux


## 实验目标

- 学习 Linux 文件系统基础
- 学习查看文件权限
- 学习 chmod 修改权限
- 理解 Linux 用户权限模型


## 实验过程


### 1. 创建目录

命令：

mkdir security


### 2. 进入目录

命令：

cd security


### 3. 创建测试文件

命令：

touch test.txt


### 4. 查看文件权限

命令：

ls -l


示例：

-rw-r--r--


权限说明：

r = read（读取）

w = write（写入）

x = execute（执行）


文件权限分为：

Owner（文件所有者）

Group（用户组）

Others（其他用户）


## 修改文件权限


### 设置全部权限

命令：

chmod 777 test.txt


结果：

-rwxrwxrwx


说明：

所有用户拥有读取、写入、执行权限。


### 设置安全权限

命令：

chmod 600 test.txt


结果：

-rw-------


说明：

只有文件所有者可以读取和修改文件。


## 实验总结


通过本次实验，我学习了 Linux 文件权限基础。

掌握：

1. 创建 Linux 文件和目录

2. 查看文件权限

3. 使用 chmod 修改权限

4. 理解 Linux 权限控制


Linux 文件权限是网络安全学习的重要基础。
