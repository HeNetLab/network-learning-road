# 06 Nmap Scan Lab

# 06 Nmap 扫描实验

---

## 1. Introduction

Nmap (Network Mapper) is a powerful network scanning tool used for network discovery, port scanning, and service detection.

Nmap（Network Mapper）是一款强大的网络扫描工具，主要用于网络发现、端口扫描和服务识别。

In this lab, I learned how to use Nmap in Kali Linux to analyze network hosts and services.

在本实验中，我学习了如何在 Kali Linux 中使用 Nmap 分析网络主机和运行服务。

---

# 2. Environment

## Operating System

Kali Linux

## Tool

Nmap 7.99

---

# 3. Check Nmap Installation

## Purpose

Verify whether Nmap is installed correctly.

确认 Nmap 工具是否正确安装。

---

## Command

```bash
nmap --version
```

---

## Result

Example output:

```
Nmap version 7.99
```

The output shows that Nmap has been installed successfully.

输出显示 Nmap 已经成功安装。

---

# 4. Localhost Scan

## Purpose

Scan the local machine and check open ports.

扫描本机，查看开放的网络端口。

---

## Command

```bash
nmap localhost
```

---

## Result

Example output:

```
PORT   STATE SERVICE
22/tcp open ssh
```

Explanation:

- 22/tcp: TCP port 22
- open: The port is available
- ssh: SSH remote management service


解释：

- 22/tcp：TCP协议22号端口
- open：端口处于开放状态
- ssh：SSH远程管理服务


---

# 5. Service Version Detection

## Purpose

Detect the service version running on the target.

检测目标运行的服务版本信息。

---

## Command

```bash
nmap -sV localhost
```

---

## Result

Example output:

```
22/tcp open ssh OpenSSH 10.3p1 Debian
```

Explanation:

Nmap can identify the service name and software version.

Nmap 可以识别服务名称以及软件版本。

---

# 6. Host Discovery

## Purpose

Discover active hosts in the local network.

发现局域网中在线的设备。

---

## Command

```bash
nmap -sn 10.0.2.0/24
```

---

## Result

Example output:

```
Nmap done: 256 IP addresses (3 hosts up)
```

Explanation:

Nmap scanned the network range and found active hosts.

解释：

Nmap扫描整个网段，并发现在线设备。

---

# 7. Port Scan

## Purpose

Scan a specific port on a target host.

扫描目标主机指定端口。

---

## Command

```bash
nmap -p 22 10.0.2.15
```

---

## Result

Example output:

```
PORT   STATE SERVICE

22/tcp open ssh
```

Explanation:

Port 22 is open and running SSH service.

解释：

22号端口开放，并运行 SSH 服务。

---

# 8. Learning Summary

## What I learned

Through this Nmap lab, I learned:

通过本次 Nmap 实验，我学习了：

- Network host discovery

  网络主机发现

- Port scanning

  端口扫描

- Service detection

  服务识别

- Understanding network exposure

  理解网络暴露面


Nmap is an important basic tool for cybersecurity learning.

Nmap 是网络安全学习中的重要基础工具。
