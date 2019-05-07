# 生物信息分析环境搭建
## 1 下载&安装 [JDK](https://www.oracle.com/technetwork/java/javase/downloads/jdk11-downloads-5066655.html)

虚拟机使用 Java 语言开发，需要提供虚拟机运行的环境。

## 2 下载&安装 虚拟机
[VMware](https://www.vmware.com/go/getworkstation-win) 或 [Virtual Box](https://www.virtualbox.org/wiki/Downloads)

在操作系统之上，提供 Linux 等其他操作系统运行的虚拟环境。

## 3 下载 Linux
[CentOS](https://www.centos.org/) 或 [Ubuntu](https://www.ubuntu.com/download/desktop)
```
Linux 内核 ------- Red Hat Enterprise Linux （商业版）
             |                |--- CentOS (Community Enterprise Operating System, RedHat 开源版）
             |--- Ubuntu
             |--- Debian
             |--- ...
```
CentOS 与 Ubuntu 是由 Linux 系统衍生出来的两个版本。

## 4 创建虚拟机

现以 VMware 为例，演示 CentOS 安装过程。

1 运行 VMware -> 2 单击 【文件】主菜单 -> 3 单击 【新建虚拟机】菜单项 

  或者 单击 【主页】 下的 【创建新的虚拟机】

4

![](https://github.com/QifengSun/bioinfomatics/blob/master/png/vmware_1.png)

5

![](https://github.com/QifengSun/bioinfomatics/blob/master/png/vmware_2.png)

6 指定待安装的操作系统

![](https://github.com/QifengSun/bioinfomatics/blob/master/png/vmware_3.png)

7 指定虚拟机文件存放位置

![](https://github.com/QifengSun/bioinfomatics/blob/master/png/vmware_4.png)

8 指定虚拟机硬盘大小上限，随着虚拟机里的文件大小动态扩容的。

![](https://github.com/QifengSun/bioinfomatics/blob/master/png/vmware_5.png)

9 单击 【自定义硬件...】

![](https://github.com/QifengSun/bioinfomatics/blob/master/png/vmware_6.png)

10 指定分配给虚拟机的内存大小

![](https://github.com/QifengSun/bioinfomatics/blob/master/png/vmware_7.png)

11 指定处理器的数量，与内核数量，以本机实际的处理器数量与内核数量为限

![](https://github.com/QifengSun/bioinfomatics/blob/master/png/vmware_8.png)

12 指定安装 Linux 的 ISO 镜像文件

![](https://github.com/QifengSun/bioinfomatics/blob/master/png/vmware_9.png)

13 配置虚拟机网络适配器的网络连接模式

![](https://github.com/QifengSun/bioinfomatics/blob/master/png/vmware_10.png)

NAT（Network Address Translation，网络地址转换)

通过虚拟的网卡（网关:192.168.43.1，DNS:192.168.43.2)，实现虚拟内网主机 (192.168.43.100, 192.168.43.101 ...) 与 外网的连接。

14 单击 【完成】

![](https://github.com/QifengSun/bioinfomatics/blob/master/png/vmware_11.png)

15 单击 【开启此虚拟机】

![](https://github.com/QifengSun/bioinfomatics/blob/master/png/CentOS_1.png)

16 指定语言

![](https://github.com/QifengSun/bioinfomatics/blob/master/png/CentOS_2.png)

17 单击 【Date & Time】修改时区

![](https://github.com/QifengSun/bioinfomatics/blob/master/png/CentOS_3.png)

![](https://github.com/QifengSun/bioinfomatics/blob/master/png/CentOS_4.png)

18 

 将时区修改为上海

![](https://github.com/QifengSun/bioinfomatics/blob/master/png/CentOS_5.png)

19 单击 【INSTALLATION DESTINATION】指定 Linux 安装的虚拟磁盘位置

![](https://github.com/QifengSun/bioinfomatics/blob/master/png/CentOS_6.png)

![](https://github.com/QifengSun/bioinfomatics/blob/master/png/CentOS_7.png)

单击 【Done】

20 单击 【NETWORK & HOSTNAME】配置虚拟主机的网卡

![](https://github.com/QifengSun/bioinfomatics/blob/master/png/CentOS_8.png)

21 单击 【OFF】->【ON】开启网卡连接

![](https://github.com/QifengSun/bioinfomatics/blob/master/png/CentOS_9.png)

单击 【Configure...】

22 单击 【IPv4 Settings】选项卡 
![](https://github.com/QifengSun/bioinfomatics/blob/master/png/CentOS_10.png)

23 虚拟主机的网卡配置修改如下

![](https://github.com/QifengSun/bioinfomatics/blob/master/png/CentOS_11.png)

单击 【Save】

24 

![](https://github.com/QifengSun/bioinfomatics/blob/master/png/CentOS_12.png)

27 

![](https://github.com/QifengSun/bioinfomatics/blob/master/png/CentOS_13.png)

28 

![](https://github.com/QifengSun/bioinfomatics/blob/master/png/CentOS_14.png)

29 

![](https://github.com/QifengSun/bioinfomatics/blob/master/png/CentOS_15.png)

30 

![](https://github.com/QifengSun/bioinfomatics/blob/master/png/CentOS_16.png)

31 

![](https://github.com/QifengSun/bioinfomatics/blob/master/png/CentOS_17.png)

32 

![](https://github.com/QifengSun/bioinfomatics/blob/master/png/CentOS_18.png)

33 

