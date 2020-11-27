# 生物信息分析环境搭建

## 1 下载&安装 

### 1.1 下载 [JDK](https://www.oracle.com/technetwork/java/javase/downloads/jdk11-downloads-5066655.html)

虚拟机使用 Java 语言开发，因此需要 JDK 提供虚拟机运行的环境。

### 1.2 添加 `JAVA_HOME` 环境变量

1 右击 桌面 【此电脑】 图标 -> 2 单击 【属性】-> 3 单击 【高级系统设置】

![](https://github.com/QifengSun/bioinfomatics/blob/master/png/java_home_1.png)

4 单击 【环境变量...】

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/java_home_2.png)

5 单击 【新建(N)...】tree

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/java_home_3.png)

6 输入【变量名】`JAVA_HOME` 变量值 `java 安装目录`

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/java_home_4.png)

关闭对话框

## 2 下载&安装 虚拟机

下载 [VMware](https://www.vmware.com/go/getworkstation-win) 或 [Virtual Box](https://www.virtualbox.org/wiki/Downloads)

在操作系统之上，提供 Linux 等其他操作系统运行的虚拟环境。


## 3 下载 Linux

下载 [CentOS](https://www.centos.org/) 或 [Ubuntu](https://www.ubuntu.com/download/desktop)

```
Linux 内核 ------- Red Hat Enterprise Linux （商业版）
             |                |--- CentOS (Community Enterprise Operating System, RedHat 开源版）
             |--- Ubuntu
             |--- Debian
             |--- ...
```

CentOS 与 Ubuntu 是由 Linux 内核衍生出来的版本。


## 4 创建虚拟机

现以 VMware 为例，演示 CentOS 安装过程。

1 运行 VMware -> 2 单击 【文件】主菜单 -> 3 单击 【新建虚拟机】菜单项 

  或者 单击 【主页】 下的 【创建新的虚拟机】


4

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/vmware_1.png)


5

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/vmware_2.png)


6 指定待安装的操作系统

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/vmware_3.png)


7 指定虚拟机文件存放位置

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/vmware_4.png)


8 指定虚拟机硬盘大小上限，随着虚拟机里的文件大小动态扩容的。

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/vmware_5.png)


9 单击 【自定义硬件...】

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/vmware_6.png)


10 指定分配给虚拟机的内存大小

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/vmware_7.png)


11 指定处理器的数量，与内核数量，以本机实际的处理器数量与内核数量为限

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/vmware_8.png)


12 指定安装 Linux 的 ISO 镜像文件

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/vmware_9.png)


13 配置虚拟机网络适配器的网络连接模式

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/vmware_10.png)

NAT（Network Address Translation，网络地址转换)模式，通过虚拟的网卡（网关:192.168.43.1，DNS:192.168.43.2)，实现虚拟内网主机 (192.168.43.100, 192.168.43.101 ...) 与 外网的连接。


14 单击 【完成】

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/vmware_11.png)

## 5 Linux 安装

1 单击 【```▶```开启此虚拟机】

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/CentOS_1.png)


2 指定语言

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/CentOS_2.png)


3 单击 【Date & Time】修改时区

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/CentOS_3.png)

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/CentOS_4.png)


4 将时区修改为上海

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/CentOS_5.png)


5 单击 【INSTALLATION DESTINATION】指定 Linux 安装的虚拟磁盘位置

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/CentOS_6.png)

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/CentOS_7.png)

单击 【Done】


6 单击 【NETWORK & HOSTNAME】配置虚拟主机的网卡

单击 【OFF】->【ON】开启网卡连接

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/CentOS_8.png)


单击 【Configure...】


7 单击 【IPv4 Settings】选项卡 

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/CentOS_9.png)

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/CentOS_10.png)


8 虚拟主机的网卡配置修改如下

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/CentOS_11.png)

单击 【Save】

9 单击 【Done】 

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/CentOS_12.png)


10 单击 【Begin Installation】

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/CentOS_13.png)


11 账户管理 

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/CentOS_14.png)

12 单击 【ROORPASSWORD】 设置 root 账户密码

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/CentOS_15.png)

root 为 Linux 系统的超级管理员账户。

单击 【Done】

13 单击 【USER CREATION】 创建用户

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/CentOS_16.png)

勾选 【√ Make this user administrator】 使该用户具有 sudo 权限。具有 sudo 权限的用户可以管理员的方式执行程序。

单击 【Done】

14 单击 【Finish configuration】

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/CentOS_17.png)


15 等待安装完毕

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/CentOS_18.png)


16 单击 【Reboot】重启虚拟机

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/CentOS_19.png)


## 6 Linux 登陆

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/CentOS_20.png)


输入用户名、密码

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/CentOS_21.png)


出现提示符 `$_` 登陆成功

![](https://github.com/QifengSun/bioinfomatics/tree/master/png/CentOS_22.png)

## 7 下载 & 安装 远程登录工具

下载 [XShell](https://www.netsarang.com/zh/xshell/) 或 [putty](http://www.putty.org/)

putty 需使用翻墙软件，如 [Latern 蓝灯](https://github.com/getlantern/lantern) 绕过IP封锁，方可从官网下载。

## 8 下载 & 安装 FTP 客户端工具

下载 [XFTP](https://www.netsarang.com/zh/xftp/) 或 [FileZilla](https://filezilla-project.org/)

## 9 远程连接配置


