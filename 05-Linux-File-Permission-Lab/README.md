Linux File Permission Lab
Linux 文件权限实验
Introduction
实验介绍

This is my fifth cybersecurity foundation lab.

这是我的第5个网络安全基础实验。

This lab focuses on Linux file permission management.

本实验主要学习 Linux 文件权限管理。

Learn how Linux controls access to files through permissions.

学习 Linux 如何通过权限控制文件访问。

Environment
实验环境

System:

Kali Linux

系统：

Kali Linux

Learning Objectives
实验目标

Learn Linux file system basics.

学习 Linux 文件系统基础。

Learn how to view file permissions.

学习如何查看文件权限。

Learn how to use chmod to modify permissions.

学习如何使用 chmod 修改文件权限。

Understand Linux user permission model.

理解 Linux 用户权限模型。

Lab Process
实验过程
1. Create Directory
1. 创建实验目录

Command:

命令：

mkdir security

Explanation:

解释：

mkdir means make directory.

mkdir 表示创建目录。

Create a directory named security.

创建一个名为 security 的文件夹。

2. Enter Directory
2. 进入实验目录

Command:

命令：

cd security

Explanation:

解释：

cd means change directory.

cd 表示切换目录。

Enter the security directory.

进入 security 文件夹。

3. Create Test File
3. 创建测试文件

Command:

命令：

touch test.txt

Explanation:

解释：

touch creates a new empty file.

touch 用于创建新的空文件。

test.txt is the name of the test file.

test.txt 是测试文件的名称。

4. View File Permission
4. 查看文件权限

Command:

命令：

ls -l

Explanation:

解释：

ls means list.

ls 表示查看文件列表。

-l shows detailed information.

-l 表示显示详细信息。

Example:

示例：

-rw-r--r--

Permission:

权限：

r = read (读取)

w = write (写入)

x = execute (执行)

Permission groups:

权限分组：

Owner (文件所有者)

Group (用户组)

Others (其他用户)

5. Write File Content
5. 写入文件内容

Command:

命令：

echo "Linux Security Learning" > test.txt

Explanation:

解释：

echo outputs text.

echo 用于输出文字。

redirects the output into the file.

表示把内容写入文件。

View content:

查看内容：

cat test.txt

Result:

结果：

Linux Security Learning

Modify File Permission
修改文件权限
6. Set Full Permission
6. 设置全部权限

Command:

命令：

chmod 777 test.txt

Explanation:

解释：

chmod means change mode.

chmod 表示修改权限。

Result:

结果：

-rwxrwxrwx

Meaning:

含义：

All users have:

所有用户拥有：

Read permission.

读取权限。

Write permission.

写入权限。

Execute permission.

执行权限。

Security Note:

安全注意：

chmod 777 gives maximum permission to all users.

chmod 777 会给予所有用户最高权限。

In real servers, avoid using 777 permission.

真实服务器环境中，应避免使用 777 权限。

7. Set Secure Permission
7. 设置安全权限

Command:

命令：

chmod 600 test.txt

Result:

结果：

-rw-------

Meaning:

含义：

Only the file owner can read and modify the file.

只有文件所有者可以读取和修改文件。

Other users have no permission.

其他用户没有权限。

Summary
实验总结

Through this Linux File Permission Lab, I learned:

通过本次 Linux 文件权限实验，我学习了：

Create Linux files and directories.

创建 Linux 文件和目录。

View file permissions.

查看文件权限。

Use chmod to modify permissions.

使用 chmod 修改文件权限。

Understand Linux user permission model.

理解 Linux 用户权限模型。

Linux file permission is an important foundation of cybersecurity.

Linux 文件权限是网络安全学习的重要基础。

This lab helps me understand Linux security management.

本实验帮助我理解 Linux 系统安全管理。
