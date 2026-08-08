# Day4 - Small Business Network Lab
# Day4 - 小型企业网络实验

## Lab Overview
## 实验简介

### English
This lab simulates a small business network environment.

A router, switch, PCs, and a server are configured to build a complete LAN network.

The goal is to practice basic network configuration, IP addressing, connectivity testing, and device management.

### 中文
本实验模拟一个小型企业网络环境。

通过配置 Router、Switch、PC 和 Server，搭建一个完整的局域网环境。

主要练习：

- 网络设备基础配置
- IP 地址规划
- 网络连通测试
- MAC 地址学习


## Network Topology
## 网络拓扑

### English

Network structure:

Router0
 |
Switch0
 / | \
PC0 PC1 Server


### 中文

网络结构：

Router0
 |
Switch0
 / | \
PC0 PC1 Server


## Devices
## 设备信息

|Device|Model|Function|
|-|-|-|
|Router0|Cisco 1941|Network routing|
|Switch0|Cisco 2960-24TT|LAN connection|
|PC0|PC-PT|Client|
|PC1|PC-PT|Client|
|Server0|Server-PT|Server|


## IP Address Plan
## IP地址规划

Network:

192.168.10.0/24


|Device|IP Address|
|-|-|
|Router0|192.168.10.1|
|Switch VLAN1|192.168.10.2|
|PC0|192.168.10.10|
|PC1|192.168.10.20|
|Server0|192.168.10.100|


## Configuration Completed
## 完成配置

English:

Completed:

- Router interface configuration
- Switch VLAN1 configuration
- PC and Server IP configuration
- Connectivity testing
- MAC address verification


中文：

完成：

- Router接口配置
- Switch VLAN1管理地址配置
- PC和Server IP配置
- 网络连通测试
- MAC地址表查看


## Testing Results
## 测试结果

English:

Ping test successful.

Command:

ping 192.168.10.100


Result:

Reply from 192.168.10.100


中文：

Ping测试成功。

测试：

ping 192.168.10.100


结果：

Reply from 192.168.10.100


说明：

网络通信正常。


## Learned Skills
## 学习收获

English:

Through this lab, I learned:

- Small business network structure
- Router and Switch configuration
- IP address planning
- Network troubleshooting
- MAC address learning


中文：

通过本实验学习：

- 小型企业网络结构
- Router和Switch基础配置
- IP地址规划
- 网络故障排查
- MAC地址学习机制


## Project Files
## 项目文件

Day4-small-business-network.pkt

topology.png

router-status.png

switch-status.png

mac-table.png

Reply-from.png


## Lab Summary
## 实验总结

English:

This lab helped me understand how a small business network is built and managed.

中文：

通过本实验，我理解了小型企业网络的组成，并完成网络设备配置和通信测试。
