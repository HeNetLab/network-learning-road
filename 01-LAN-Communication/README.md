# 01 LAN Communication

# 01 局域网通信实验


## Objective / 实验目标


Build a simple Local Area Network (LAN) using Cisco Packet Tracer.

使用 Cisco Packet Tracer 搭建一个简单的局域网环境。


Learn how computers communicate through a network switch.

学习计算机如何通过交换机进行网络通信。



---

# Network Topology / 网络拓扑


The network contains:

- PC0
- PC1
- PC2
- Server0
- Cisco 2960 Switch


网络设备包括：

- PC0
- PC1
- PC2
- Server0
- Cisco 2960 交换机



Topology:


```
                    Switch0

        /            |            |            \

     Fa0/1        Fa0/2        Fa0/3        Fa0/4

       |             |             |             |

      PC0           PC1        Server0          PC2

```


Description:

All devices are connected through a switch to build a Local Area Network.

所有设备通过交换机连接，组成一个局域网。



---

# Network Devices / 网络设备


## PC (Personal Computer)


A PC is used to send and receive network data.

电脑用于发送和接收网络数据。



## Switch


A switch connects multiple devices in the same LAN.

交换机用于连接同一个局域网中的多个设备。


A switch learns MAC addresses and forwards data based on MAC addresses.

交换机会学习 MAC 地址，并根据 MAC 地址进行数据转发。



## Server


A server provides network services for other devices.

服务器为其他设备提供网络服务。



---

# IP Configuration / IP地址配置


## PC0

IPv4 Address:

```
192.168.1.10
```


Subnet Mask:

```
255.255.255.0
```



## PC1

IPv4 Address:

```
192.168.1.20
```


Subnet Mask:

```
255.255.255.0
```



## Server0

IPv4 Address:

```
192.168.1.100
```


Subnet Mask:

```
255.255.255.0
```



## PC2

IPv4 Address:

```
192.168.1.30
```


Subnet Mask:

```
255.255.255.0
```



All devices are in the same network:

```
192.168.1.0/24
```


所有设备属于同一个网段：

```
192.168.1.0/24
```



---

# Communication Test / 通信测试


Use ping command to test network connectivity.


使用 ping 命令测试网络连接。



Command:


```bash
ping 192.168.1.100
```



Result:


PC0 successfully received reply from Server0.


结果：

PC0 成功收到 Server0 返回的数据。


The LAN communication is working correctly.

说明局域网通信正常。



---

# ARP Learning / ARP 地址解析


ARP (Address Resolution Protocol) maps an IP address to a MAC address.

ARP 协议用于通过 IP 地址查询对应的 MAC 地址。



Process:


```
IP Address

↓

ARP Request

↓

MAC Address

↓

Data Communication
```



过程：


```
IP 地址

↓

ARP 请求

↓

MAC 地址

↓

数据通信
```



Command:


```bash
arp -a
```



Purpose:


View the relationship between IP addresses and MAC addresses.


作用：

查看 IP 地址和 MAC 地址之间的对应关系。



---

# MAC Address Learning / MAC地址学习


The switch automatically learns MAC addresses from connected devices.


交换机会自动学习连接设备的 MAC 地址。



Command:


```bash
show mac address-table
```



Example result:


```
MAC Address          Port

PC0 MAC              Fa0/1

PC1 MAC              Fa0/2

Server MAC           Fa0/3

PC2 MAC              Fa0/4
```



The switch has learned four connected devices.


交换机已经学习到了四台设备的信息。



---

# Experiment Result / 实验结果


The LAN communication experiment was completed successfully.


本次局域网通信实验成功完成。



Learning Results:


- Built a simple LAN topology
- Configured IP addresses
- Tested connectivity with Ping
- Learned ARP protocol
- Checked switch MAC address table


学习成果：


- 搭建简单局域网拓扑
- 配置 IP 地址
- 使用 Ping 测试通信
- 理解 ARP 协议
- 查看交换机 MAC 地址表



---

# Key Concepts / 核心知识


- LAN
- IP Address
- Subnet Mask
- MAC Address
- ARP
- Switch
- Ping
- Network Communication



核心知识：


- 局域网
- IP 地址
- 子网掩码
- MAC 地址
- ARP 协议
- 交换机
- Ping 测试
- 网络通信



---

# Hong Kong IT Terminology / 香港 IT 用語


## Network Terms / 網絡術語


LAN

區域網絡


Network

網絡


IP Address

IP 地址


Subnet Mask

子網掩碼


MAC Address

MAC 地址



---

## Hardware Terms / 硬件術語


PC

電腦


Switch

交換機


Server

伺服器


Router

路由器



---

## Configuration Terms / 設定術語


Configuration

設定


Configure

設定 / 配置


Interface

介面


Port

接口



---

## Troubleshooting Terms / 故障排查術語


Ping Test

Ping 測試


Connectivity

連接情況


Network Issue

網絡問題


Troubleshooting

故障排查



---

# 香港 IT 實驗總結


今次實驗學識咗：


1. 點樣建立一個簡單嘅區域網絡。


2. 點樣使用 Switch 連接多部設備。


3. 點樣設定 IP 地址。


4. 點樣使用 Ping 測試網絡連接。


5. 點樣查看 Switch 學習到嘅 MAC 地址。


