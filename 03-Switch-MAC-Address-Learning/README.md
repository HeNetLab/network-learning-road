# 03 Switch MAC Address Learning
# 实验03：交换机MAC地址学习


## 1. Experiment Purpose / 实验目的

Learn how a switch learns MAC addresses.

学习交换机如何学习 MAC 地址。

Understand how the switch forwards data through the MAC address table.

理解交换机如何通过 MAC 地址表转发数据。


## 2. Experiment Environment / 实验环境

Software:
Cisco Packet Tracer

Devices:
Cisco 2960 Switch
PC0
PC1


## 3. Network Topology / 网络拓扑

PC0 -------- Switch0 -------- PC1


IP Configuration / IP配置：

PC0:
IP Address: 192.168.1.10
Subnet Mask: 255.255.255.0


PC1:
IP Address: 192.168.1.20
Subnet Mask: 255.255.255.0



## 4. Experiment Steps / 实验步骤


Step 1: Configure PC IP Address

步骤1：配置电脑IP地址


PC0:
192.168.1.10


PC1:
192.168.1.20



Step 2: Test Network Connection

步骤2：测试网络连接


Command:

ping 192.168.1.20


Result:

Reply from 192.168.1.20


两台电脑通信成功。



Step 3: Check Switch MAC Address Table

步骤3：查看交换机MAC地址表


Command:

enable


Meaning:

Enter privileged mode.

作用：

进入交换机管理员模式。


Command:

show mac address-table


Meaning:

Display MAC addresses learned by switch.

作用：

查看交换机学习到的 MAC 地址。



## 5. Result / 实验结果


Example:

MAC Address        Type        Port

0001.6471.89cb     Dynamic     Fa0/1

0060.5c39.e160     Dynamic     Fa0/2


The switch learned the MAC addresses of connected devices.

交换机成功学习连接设备的 MAC 地址。



## 6. Knowledge Summary / 知识总结


MAC Address:

A unique hardware address of a network device.

MAC地址：

网络设备唯一的硬件地址。


Switch Learning:

The switch learns the source MAC address from data frames.

交换机通过数据帧学习源 MAC 地址。


MAC Address Table:

The switch uses the MAC table to forward data.

交换机通过 MAC 地址表转发数据。



## 7. What Can I Do After Learning This? / 学会后可以做什么？


After learning MAC address tables, you can:

学习 MAC 地址表后，可以：


- Understand how switches work.
- Troubleshoot LAN communication problems.
- Configure and maintain enterprise networks.


- 理解交换机工作原理。
- 排查局域网通信问题。
- 进行企业网络维护。



## 8. Experiment Files / 实验文件


03-Switch-MAC-Address-Learning.pkt

topology.png

ping-test.png

mac-address-table.png

README.md
