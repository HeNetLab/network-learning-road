# Linux File Permission Lab

## Introduction

This is my first Linux security practice lab.

这是我的第一个 Linux 网络安全基础实验。

## Environment

System:
Kali Linux

## Learning Objectives

- Understand Linux file system
- Learn file permission
- Learn chmod command
- Understand user privilege

学习目标：

- 了解 Linux 文件系统
- 掌握 Linux 文件权限
- 学习 chmod 权限修改命令
- 理解用户权限管理


## Practice Process

Completed experiments:

1. Create directory

创建目录：

mkdir security


2. Create file

创建文件：

touch test.txt


3. View file permission

查看文件权限：

ls -l


4. Modify permission

修改权限：

chmod 600 test.txt

chmod 777 test.txt


## Permission Understanding

Example:

-rw-r--r--

Meaning:

- r = read（读取权限）
- w = write（写入权限）
- x = execute（执行权限）


Permission:

Owner（文件所有者）

Group（用户组）

Others（其他用户）


## Summary

Through this lab, I learned the basic Linux file permission system.

通过本次实验，我掌握了 Linux 文件权限基础，为后续网络安全学习打下基础。
