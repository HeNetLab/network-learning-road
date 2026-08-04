
# 02 Switch Basic Configuration

# 实验02：交换机基础配置


## 1. Experiment Purpose / 实验目的

Learn basic Cisco switch configuration.

学习 Cisco 交换机基础配置。


Configure switch hostname and management IP.

配置交换机名称和管理IP。


Test network connectivity using ping.

使用 ping 测试网络连通性。


---

## 2. Environment / 实验环境

Tool:

Cisco Packet Tracer


Device:

- Cisco Catalyst 2960 Switch
- PC-PT


设备：

- Cisco Catalyst 2960 交换机
- PC电脑


---

## 3. Network Topology / 网络拓扑

PC0 ---- Switch0


PC0 IP Address:

192.168.1.10


Switch VLAN 1 IP Address:

192.168.1.2


---

## 4. Configuration Commands / 配置命令


### 1) Enter privileged mode

进入管理员模式


Command:

enable


Function:

Enter switch administrator mode.

作用：

进入交换机管理员模式。


---

### 2) Enter configuration mode

进入配置模式


Command:

conf t


Function:

Enter global configuration mode.

作用：

进入全局配置模式。


---

### 3) Change hostname

修改交换机名称


Command:

hostname SW1


Function:

Change the switch name for management.

作用：

修改交换机名称，方便管理。


---

### 4) Configure VLAN 1 interface

配置 VLAN 1 管理接口


Command:

interface vlan 1


Function:

Enter VLAN 1 management interface.

作用：

进入 VLAN 1 管理接口。


---

### 5) Configure IP address

配置IP地址


Command:

ip address 192.168.1.2 255.255.255.0


Function:

Assign IP address to switch management interface.

作用：

给交换机管理接口配置IP地址。


---

### 6) Enable interface

开启接口


Command:

no shutdown


Function:

Enable the interface.

作用：

开启接口。


---

### 7) Save configuration

保存配置


Command:

write


Function:

Save current configuration.

作用：

保存当前配置。


---

## 5. Connectivity Test / 网络测试


Command:

ping 192.168.1.2


Result:

Reply from 192.168.1.2


The connection is successful.

网络连接成功。


---

## 6. Learning Summary / 学习总结


Learned basic Cisco IOS commands.

学习了 Cisco IOS 基础命令。


Learned how to configure switch management IP.

学习了如何配置交换机管理IP。


Understood the basic workflow of network device configuration.

理解了网络设备配置的基本流程。


---

## 7. Experiment Files / 实验文件


- 02-Switch-Basic-Configuration.pkt

- topology.png

- switch-config.png

- ping-test.png





