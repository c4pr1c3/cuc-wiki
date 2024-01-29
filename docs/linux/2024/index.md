# Linux系统与网络管理

## 一、课程基本信息

<img align="right" src="../img/url-of-linux-wiki.png"/>

* 课程编号：2121030017
* 英文名称：Linux System and Network Management
* 授课对象：网络空间安全
* 开课学期：4
* 学分/学时：1.5/32（课内16学时，实验上机16学时）
* 先修课程：计算机导论，计算机安全与维护
* 教学方式：课内（线上）讲授，上机实验
* [详细教学日历](calendar.md)
* [本学期课程考核规则](homework.md)
* [2021 年完整课程视频回放](https://www.bilibili.com/video/BV1Hb4y1R7FE)

### 课程简介

Linux网络操作系统支持多用户与多任务，近年来发展迅速，已经成为主流操作系统之一，具有十分广泛的应用。本课程以Linux网络操作系统为范例，以理论联系实际的教学方法，系统学习网络操作系统的使用以及网络系统和网络服务构建的相关知识，并通过课程实践，培养学生的实际技能。主要包括Linux安装、系统管理与网络基础；DHCP、WEB、FTP、Samba、NFS、DNS等网络服务的基本原理与服务器配置与应用。通过本课程学习，使学生掌握基于Linux网络操作系统进行网络系统与服务的部署、应用、管理的相关知识和技能。

## 二、课程教学目的和要求

Linux是网络应用领域中广泛使用的一种主流操作系统。通过本课程学习，使学生掌握基于Linux网络操作系统进行网络系统与服务的布署、应用、管理的相关知识和技能，为网络系统管理、云计算及服务器应用开发等奠定基础。

## 三、教学内容与学时分配

第一章： Linux基础（2学时）

* 概述：发行版、开源社区与文化、内核版本历史、LSB(Linux Standard Base)、CGL(Carrier Grade Linux)、Linux Foundation等
* 操作系统安装：物理机安装、虚拟机安装、系统分区、无人值守安装等
* 内置帮助系统的使用：man、--help、-h
* 命令行使用：shell家族、自动补全、重复命令输入等bash常用快捷键、文本编辑与查看（echo、cat、less、vim、sort、uniq、wc等）
* SSH与远程服务器管理：免密登录、SSH跳板与堡垒主机、SSH服务器安全加固

[在线查看课件](https://c4pr1c3.github.io/LinuxSysAdmin/chap0x01.md.html)

第二章：Linux服务器系统使用基础（2学时）

* 文件的压缩与解压缩：tar、gz、zip、gzip、7z等、跨平台压缩文件的中文乱码问题等
* 软件包管理：安装、升级、卸载、源码下载与安装
* 文件管理：find、grep、sed等命令的使用
* 进程管理：ps、kill等命令的使用
* 目录结构：man hier、ls
* 网络调试：ethtool、ip、ifconfig、arp、traceroute、netstat、route、/etc/hosts、/etc/resolv.conf、tcpdump等

[在线查看课件](https://c4pr1c3.github.io/LinuxSysAdmin/chap0x02.md.html)

第三章：Linux服务器系统管理基础（2学时）

* 用户/组与权限管理：su与sudo、passwd、adduser/useradd、groupadd/addgroup、usermod、getfacl/setfacl等命令的使用
* 文件系统与存储管理：文件系统类型与格式化、磁盘分区、存储设备与文件系统挂载（开机自动挂载、网络文件系统挂载、iso文件挂载等）、基于LVM（逻辑分卷管理）的分区容量动态调整
* 文件备份与恢复（文件和目录属主信息的保存）等
* 开机自启动项管理：系统加载流程（[Systemd](https://wiki.archlinux.org/index.php/systemd_(%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87) )、[LSBInitScripts](https://wiki.debian.org/LSBInitScripts) )
* 配置每天自动安装安全更新

[在线查看课件](https://c4pr1c3.github.io/LinuxSysAdmin/chap0x03.md.html)

第四章：shell脚本编程基础（2学时）

* 开发和调试环境搭建
* 基本语法：shell版本、变量定义、环境变量、过程（函数）、条件语句、循环、数值计算、数组、子进程等
* 实例讲解：校园网自动联网bash脚本

[在线查看课件](https://c4pr1c3.github.io/LinuxSysAdmin/chap0x04.md.html)

第五章：Web服务器（2学时）

* Web服务基本概念：HTTP请求处理的生命周期
* 主流WEB服务器：apache 1.x/2.x、nginx（衍生发行版：[OpenResty](https://github.com/openresty/openresty)、[Kong](https://github.com/Mashape/kong)、[Tengine](http://tengine.taobao.org/)）
* 用curl和nginx重新认识和学习HTTP协议

[在线查看课件](https://c4pr1c3.github.io/LinuxSysAdmin/chap0x05.md.html)

第六章：网络资源共享（1学时）

* FTP服务概述及FTP服务器配置
* NFS服务概述及NFS服务器配置
* Samba服务概述及Samba服务器安装与配置

[在线查看课件](https://c4pr1c3.github.io/LinuxSysAdmin/chap0x06.md.html)

第七章：DHCP与DNS服务（1学时）

* DHCP服务概述
* DHCP基本原理
* DHCP服务器安装配置
* DNS服务概述
* DNS服务器配置

[在线查看课件](https://c4pr1c3.github.io/LinuxSysAdmin/chap0x07.md.html)

第八章：DevOps文化、运维自动化与持续部署（4学时）

* 发布管理：开发环境、测试环境与生产环境的一致性（代码、数据、网络、系统运行时、依赖的lib等）、上线与回滚
* 主流技术工具链：git（github/gitlab）、[ansible](https://www.ansible.com/)（puppet、chef、salt等）、docker（dockerfile/k8s/dockerhub）、openstack（KVM、Xen）、openvswitch、tcpreplay

[在线查看课件](https://c4pr1c3.github.io/LinuxSysAdmin/chap0x08.md.html) | [PXE](https://c4pr1c3.github.io/LinuxSysAdmin/PXE.md.html) | [ansible](https://c4pr1c3.github.io/LinuxSysAdmin/ansible.md.html) 

## 四、作业、实践环节

- H1 [主流 Linux 发行版初体验（2学时）：本地实验环境和云实验环境](https://c4pr1c3.github.io/LinuxSysAdmin/chap0x01.exp.md.html) ⭐️⭐️
- H2 [Linux命令行使用基础（2学时）：本地实验环境和云实验环境](https://c4pr1c3.github.io/LinuxSysAdmin/chap0x02.exp.md.html) ⭐️⭐️
- H3 [开机自启动项目管理与网络故障排查](https://c4pr1c3.github.io/LinuxSysAdmin/chap0x03.exp.md.html)（2学时）⭐️⭐️
- H4 [shell脚本编程练习基础（2学时）：文本处理（考察去重、统计、排序等操作）、文件批量重命名（简单重命名规则、复杂重命名规则）](https://c4pr1c3.github.io/LinuxSysAdmin/chap0x04.exp.md.html) ⭐️⭐️⭐️⭐️⭐️
- H5 [支持反向代理、流量控制、关键词过滤等功能的高级Web服务器配置（2学时）](https://c4pr1c3.github.io/LinuxSysAdmin/chap0x05.exp.md.html) ⭐️⭐️⭐️⭐️
- H6 【**提交到私有作业仓库**】[shell脚本编程练习进阶（2学时）：FTP、NFS、DHCP、DNS、Samba服务器的自动安装与自动配置](https://c4pr1c3.github.io/LinuxSysAdmin/chap0x06.exp.md.html) ⭐️⭐️⭐️⭐️⭐️
- H7 【**提交到私有作业仓库**】使用ansible技术重构FTP、NFS、DHCP、DNS、Samba服务器的自动安装与自动配置（2学时） ⭐️⭐️⭐️⭐️⭐️
- H8 【**提交到私有作业仓库**】使用容器技术重构FTP、NFS、DHCP、DNS、Samba服务器的自动安装与自动配置（2学时）⭐️⭐️⭐️⭐️

| **难度等级** | 说明                                                     |
| :--:         | --                                                       |
| ⭐️           | 照葫芦画瓢，没有坑。                                     |
| ⭐️⭐️         | 照猫画虎，可能有小坑。                                   |
| ⭐️⭐️⭐️       | 有较为详细的参考资料，但坑也不少，考察自己动手搜索能力。 |
| ⭐️⭐️⭐️⭐️     | 参考资料较多，但需要提高信息检索和甄别能力。             |
| ⭐️⭐️⭐️⭐️⭐️   | 偏综合能力训练，编程能力要求中等偏上。                   |

## 五、建议教材

所有课件的源代码均已开源在[Github - c4pr1c3/LinuxSysAdmin](https://github.com/c4pr1c3/LinuxSysAdmin)

## 六、参考资料

* [Linux Foundation Certified System Administrator](https://linuxacademy.com/linux/training/course/name/linux-foundation-certified-systems-administrator)
* [Red Hat System Administration I RH124](https://www.redhat.com/en/services/training/rh124-red-hat-system-administration-i)
* [Red Hat System Administration II with RHCSA exam](https://www.redhat.com/en/services/training/rh135-red-hat-system-administration-ii-rhcsa-exam)
* [Red Hat Certified System Administrator (RHCSA) exam EX200](https://www.redhat.com/en/services/training/ex200-red-hat-certified-system-administrator-rhcsa-exam)
* [BASH Programming - Introduction HOW-TO](http://tldp.org/HOWTO/Bash-Prog-Intro-HOWTO.html)
* [Bash Reference Manual from gnu.org](https://www.gnu.org/software/bash/manual/html_node/index.html)
* [Shell Style Guide by Google Inc.](https://google.github.io/styleguide/shell.xml)
* [UNIX TOOLBOX: a collection of Unix/Linux/BSD commands and tasks which are useful for IT work or for advanced users](http://cb.vu/unixtoolbox.xhtml)
* [鸟哥的Linux私房菜](http://cn.linux.vbird.org/)

