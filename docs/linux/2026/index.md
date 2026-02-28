# Linux系统与网络管理

## 一、课程基本信息

* 课程编号：2121030017
* 英文名称：Linux System and Network Management
* 授课对象：网络空间安全
* 开课学期：4
* 学分/学时：1.5/32（课内16学时，实验上机16学时）
* 先修课程：计算机导论，计算机安全与维护
* 教学方式：课内讲授，上机实验
* 课件仓库：[Github - c4pr1c3/Linux4AI](https://github.com/c4pr1c3/Linux4AI)

### 课程简介

Linux 在服务器、云原生与安全运维领域具有事实标准地位。本课程以现代 Linux 使用与管理为主线，强调理论联系实际，围绕环境构建、命令行与包管理、权限与用户管理、系统排障与可观测性、存储与网络配置、自动化与可复现（Shell/Docker/Ansible）、服务交付与安全基线等内容展开。通过课内讲授与上机实践，培养学生在真实环境中完成部署、运维、排障与安全审计的能力。

## 二、课程教学目的和要求

通过本课程学习，使学生掌握基于 Linux 操作系统进行环境搭建、系统管理、网络配置、服务交付、自动化运维与安全加固的相关知识与技能，为网络系统管理、云计算与安全工程实践打下基础。

## 三、教学内容与学时分配

### 课程知识图谱

```markmap
# Linux系统与网络管理

## 典型任务场景

### 搭建个人开发环境并实现远程开发

- 关键能力点
  - 配置 WSL/终端与基础工具链
  - 生成与管理 SSH 密钥
  - 编写可维护的 SSH 配置
- 关键知识点
  - WSL 2 与 Linux 发行版概念
  - ssh-keygen / ssh-copy-id / ~/.ssh/config
  - 最小权限与 sudo 使用边界

### 在服务器上进行快速巡检与日志取证

- 关键能力点
  - 使用管道组合命令完成筛选与统计
  - 提取关键字段并形成结论
  - 记录可复现的命令流与结果
- 关键知识点
  - STDIN/STDOUT/STDERR / 重定向 / 管道
  - grep / awk / sort / uniq / head
  - 日志格式与字段含义

### 处理（服务异常/端口占用/连接失败）等典型故障

- 关键能力点
  - 定位进程、信号与资源占用
  - 定位端口占用并安全终止
  - 基于日志还原故障现场
- 关键知识点
  - ps / top / kill(信号语义)
  - ss / lsof
  - systemctl / journalctl
```


### 第零单元：Linux 概论

*   [Linux 概论](https://c4pr1c3.github.io/linux4ai/courseware/unit00-intro/slides/00-intro2linux.html)：AI 时代的 Linux, 历史与哲学, 发行版(Ubuntu/LTS), CLI 价值

### 第一单元：环境构建与 CLI 生存指南（4学时）

*   [WSL, SSH & 远程开发](https://c4pr1c3.github.io/linux4ai/courseware/unit01-env-cli/slides/01-wsl-ssh.html)：WSL2, Linux 发行版, 权限管理(root/sudo), SSH 密钥认证
*   [命令行的艺术与技术](https://c4pr1c3.github.io/linux4ai/courseware/unit01-env-cli/slides/02a-cli-survival.html)：Shell, 管道/重定向, grep/awk, find, xargs
*   [软件包管理艺术与技术](https://c4pr1c3.github.io/linux4ai/courseware/unit01-env-cli/slides/02b-package-mgmt.html)：apt/dpkg, 镜像源配置, 依赖管理, 软件安装与卸载

### 第二单元：系统运维与排障（4学时）

*   [权限, 访问控制列表 & 文件系统结构](https://c4pr1c3.github.io/linux4ai/courseware/unit02-sys-debug/slides/03a-permissions.html)：UGO 权限模型, ACL, umask, 目录权限
*   [用户与权限管理](https://c4pr1c3.github.io/linux4ai/courseware/unit02-sys-debug/slides/03b-user-admin.html)：/etc/passwd, useradd/usermod, sudoers, 最小权限原则
*   [系统可观测性 & 故障排查](https://c4pr1c3.github.io/linux4ai/courseware/unit02-sys-debug/slides/04a-process-debug.html)：journalctl, ps/top, kill 信号, ss/netstat, 故障排查
*   [存储管理基础](https://c4pr1c3.github.io/linux4ai/courseware/unit02-sys-debug/slides/04b-storage.html)：分区(fdisk/gdisk), 格式化(mkfs), 挂载(mount), /etc/fstab, LVM
*   [网络配置管理](https://c4pr1c3.github.io/linux4ai/courseware/unit02-sys-debug/slides/04c-network-config.html)：iproute2, Netplan, DNS, 路由表

### 第三单元：自动化与可复现（4学时）

*   [脚本编程: 从单行脚本到生产级](https://c4pr1c3.github.io/linux4ai/courseware/unit03-automation/slides/05a-shell-scripting.html)：Shell 脚本, set -euo pipefail, 幂等性, 模块化
*   [Docker 容器技术入门](https://c4pr1c3.github.io/linux4ai/courseware/unit03-automation/slides/05b-docker-intro.html)：容器 vs 虚拟机, Image/Container, docker run/exec, 镜像加速
*   [代码即基础设施：Ansible 基础](https://c4pr1c3.github.io/linux4ai/courseware/unit03-automation/slides/05c-ansible-minimal.html)：IaC, 无 Agent, 幂等性, Inventory, Playbook

### 第四单元：服务交付与安全基线（4学时）

*   [Nginx, 反向代理 & 日志](https://c4pr1c3.github.io/linux4ai/courseware/unit04-service-sec/slides/07-web-service.html)：反向代理, 负载均衡, Nginx 配置, Access Log
*   [安全基线 & AI 辅助运维](https://c4pr1c3.github.io/linux4ai/courseware/unit04-service-sec/slides/08-security-ai.html)：最小权限原则, SSH 加固, AI 辅助脚本审计, 幻觉风险

## 四、作业、实践环节

*   [Lab 01: 环境构建与 CLI 初探](https://c4pr1c3.github.io/linux4ai/courseware/unit01-env-cli/labs/lab01-setup.html) ⭐️⭐️
*   [Lab 02: 权限迷宫与系统排障](https://c4pr1c3.github.io/linux4ai/courseware/unit02-sys-debug/labs/lab02-debug.html) ⭐️⭐️⭐️
*   [Lab 03: 自动化运维实战](https://c4pr1c3.github.io/linux4ai/courseware/unit03-automation/labs/lab03-automation.html) ⭐️⭐️⭐️⭐️
*   [Lab 03b: Docker 容器实战](https://c4pr1c3.github.io/linux4ai/courseware/unit03-automation/labs/lab03b-docker.html) ⭐️⭐️⭐️
*   [Lab 04: 服务交付与安全审计](https://c4pr1c3.github.io/linux4ai/courseware/unit04-service-sec/labs/lab04-service.html) ⭐️⭐️⭐️⭐️⭐️

| **难度等级** | 说明                                                                   |
| :--:         | --                                                                     |
| ⭐️           | 跟随步骤可完成，主要练基本操作；可用 AI 解释概念/命令含义。             |
| ⭐️⭐️         | 需要根据环境差异做少量调整；可用 AI 辅助定位报错点并给出修复思路。       |
| ⭐️⭐️⭐️       | 需要组合多种工具完成任务并形成结论；可用 AI 生成候选命令，但必须验证。   |
| ⭐️⭐️⭐️⭐️     | 开放性更强，要求你设计方案与权衡安全/可复现；可用 AI 做方案迭代与代码审计。 |
| ⭐️⭐️⭐️⭐️⭐️   | 综合项目式交付，强调端到端验证、审计与复盘；AI 深度参与，但风险由你兜底。 |

## 五、建议教材

本课程以课件与实验指导为主，配合权威手册与官方文档进行学习与检索。

## 六、参考资料

* [Red Hat Certified System Administrator (RHCSA) exam EX200](https://www.redhat.com/en/services/training/ex200-red-hat-certified-system-administrator-rhcsa-exam)
* [Bash Reference Manual from gnu.org](https://www.gnu.org/software/bash/manual/html_node/index.html)
* [Shell Style Guide by Google Inc.](https://google.github.io/styleguide/shell.xml)
* [UNIX TOOLBOX: a collection of Unix/Linux/BSD commands and tasks which are useful for IT work or for advanced users](http://cb.vu/unixtoolbox.xhtml)
* [鸟哥的Linux私房菜](http://cn.linux.vbird.org/)
