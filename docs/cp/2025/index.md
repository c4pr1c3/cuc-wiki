# 2025 年教学计划

## 课程基本信息

* 主讲教师：黄玮、安靖
* 课程主题：网络空间安全两年半专业课综合运用和实践
* 实验准备：自备电脑，
* 上课方式：线下集中实践+分组学习+自行组队完成大作业+集中报告

## 课程目标

1. 了解网络攻防相关法律法规，理解网络攻防的基本概念、基本原理和基本方法。
2. 掌握网络攻防的基本技术，包括红队技术（例如：信息收集、端口扫描、服务识别、漏洞扫描、漏洞利用）和蓝队技术（例如：入侵检测、入侵取证、应急响应等）。
3. 理解网络靶场的概念，掌握网络靶场的搭建方法、演练方案的设计和实施方法。

## 课程内容

本实践课程以 `团队实践训练` 任务形式开展。顾名思义，`团队实践训练` 采取同学们自由组队 **分组完成** 方式，每个小组至多允许 *6* 人，建议 **4** 人最佳。

本次课程实践由 2 个阶段的任务共同组成，分别是： `基础团队实践训练` 和 `进阶团队实践训练`。

### 1. 基础团队实践训练

团队分工跟练复现完成 [网络安全(2021) 综合实验](https://www.bilibili.com/video/BV1p3411x7da/) 。无论团队由多少人所组成，以下按本次实践训练所涉及到的人员能力集合划分了以下团队角色。一人至少承担一种团队角色，老师将按照该角色的评价标准进行 `基于客观事实的主观评价` 。

* 红队：需完成漏洞存在性验证和漏洞利用。
* 蓝队威胁监测：漏洞利用的持续检测和威胁识别与报告。
* 蓝队威胁处置：漏洞利用的缓解和漏洞修复（源代码级别和二进制级别两种）。

上述能力的基本评分原则参考“道术器”原则：最基础要求是能够跟练并复现 [网络安全(2021) 综合实验](https://www.bilibili.com/video/BV1p3411x7da/) 中演示实验使用到的工具；进阶标准是能够使用课程视频中 **未使用** 的工具或使用编程自动化、甚至是智能化的方式完成漏洞攻击或漏洞利用行为识别与处置。

### 2. 进阶团队实践训练

设计不同于 [网络安全(2021) 综合实验](https://www.bilibili.com/video/BV1p3411x7da/) 中的典型企业三层网络架构的攻防场景，评分时将从靶标所包含漏洞的差异性、漏洞利用的复杂性、网络拓扑的差异性、网络拓扑的复杂性、ATT&CK 技术点的覆盖数量、蓝队的威胁监测与处置的复杂性等方面进行评分。

#### 涉及到的主要知识点和技能点

- 虚拟机软件（推荐 `Virutalbox`）的安装和基本使用
- Ubuntu 系统的使用
- Kali Linux 系统的使用
- 在不同 Linux 发行版里的 Docker 容器的安装和基本使用
- 通过 Dockerfile 构建靶标镜像
- 通过 Docker Compose 部署靶标环境
- 基于 [Vulfocus](https://github.com/c4pr1c3/ctf-games/tree/master/fofapro/vulfocus) 的漏洞复现
- 基于 [Vulfocus](https://github.com/c4pr1c3/ctf-games/tree/master/fofapro/vulfocus) 的靶场搭建
- 外网渗透测试：信息收集、端口扫描、服务识别、漏洞扫描、漏洞存在性验证、漏洞利用
- Metasploit 及其他开源自动化攻击框架的使用
- 内网渗透测试：信息收集、端口扫描、服务识别、网络拓扑发现、漏洞扫描、漏洞存在性验证、漏洞利用
- 使用 Git 进行团队协作
- 搜索引擎的使用
- AI Copilot 的使用
- 自动化攻击程序的编写
- 入侵检测系统的安装与使用
- 入侵取证
- 漏洞利用缓解
- 漏洞修复
- 规范的技术文档撰写能力
- ATT&CK 知识库的使用

## 成绩评定

* 按照团队实践训练的总体完成度情况，通过团队的现场口头报告情况和提交的书面报告质量进行综合评定。
* 总成绩 = `口头报告` * 40% + `书面报告` * 50% + `考勤记录` * 10% 。
* `口头报告` 现场报告完毕后，老师将根据现场报告的内容和团队成员的表现情况给予团队总体表现评分。团队成员现场完成团队分数到个人评分的分配和确认。举例，团队总体获得评分 90 ，团队由 6 人组成，此时可以用于分配给团队内个人的评分总数计算公式为：团队总分 * 团队人数 = 90 * 6 = 540 = 团队可分配总分。最终确认的个人评分分配方案需确保 `团队个人评分之和` = `团队可分配总分` 。
* `书面报告` 书面报告的质量将根据书面报告的内容、排版、撰写质量、撰写规范、代码规范、`Git 使用规范性` 等方面进行评分。
* `基础团队实践训练` 和 `进阶团队实践训练` 各有一次独立的 `口头报告` 和 `书面报告` 评分，两次评分采用平均分方式计入期末成绩。
* `考勤记录` 考勤记录将根据同学们的出勤情况进行评分。初始考勤为满分 10 分，无故缺勤或早退 1 次扣 1 分，迟到 1 次扣 0.5 分，以此类推，扣完为止。

## 难度级别说明

- ⭐️⭐️⭐️⭐️⭐️ 为最高难度级别，对团队成员的技术能力要求最高，需要团队成员具备很强的自主学习与动手实践能力、团队协作能力和举一反三能力。
- ⭐️⭐️⭐️⭐️ 为较高难度级别，对团队成员的技术能力要求较高，需要团队成员具备较强的自主学习与动手实践能力、团队协作能力和集成创新或微调改造能力。
- ⭐️⭐️⭐️ 为中等难度级别，对团队成员的技术能力要求一般，需要团队成员具备基本的自主学习与动手实践能力、团队协作能力和扎实的故障排查能力。
- ⭐️⭐️ 为较低难度级别，对团队成员的技术能力要求较低，需要团队成员具备基本的自主学习与动手实践能力、团队协作能力和基本的故障排查能力。
- ⭐️为最低难度级别，以 `跟练和复现` 形式为典型代表，且在操作过程中使用的工具软件具有较强的容错健壮性、较高的自动化水平甚至具备一定的自主智能性。

## 口头报告要求

* 每个小组 20 分钟以内的现场报告时间，包括团队成员的分工、完成情况、遇到的问题和解决方案等。
* 接受现场老师和同学们的提问，回答问题，解释团队的工作成果原理、团队成员的贡献，半小时左右。
* 同学们微信小窗联系授课老师申请安排现场口头报告时间，报告的先后顺序以同学们完整书面报告和答辩 PPT 提交到 `git` 仓库的提交时间为排序依据。
* 现场口头报告后老师提出的修改意见，同学们需要在书面报告中进行修改，并在后续的 `git` 提交后，通过 `commit message` 或 `git 网页版的评论功能` 归纳概述修改落实情况或未修改原因，以便最终评分。

## 书面报告要求

* 实践训练过程中产生的文档、代码均可以采用 Github/[Gitlab](https://git.cuc.edu.cn)/Gitee 的方式管理（这是一个鼓励和支持的作业完成过程建议，有助于提高印象分哦～）；
* 结课材料，统一用zip格式打包并提交到学校畅课平台指定作业模块（后续在课程微信群、畅课平台课程公告模块进行通知，注意查看）。附件命名规范：`姓名1_姓名2_姓名3_姓名4_姓名5_姓名6_作业题目.zip`；
    * 姓名先后顺序按照 `口头报告` 环节确认的个人得分，从高到低、从左到右依次排列；
    * 所有文档统一采用 **markdown** 书写，建议参照 [基于 Markdown 的中文文档排版规范](https://xie.infoq.cn/article/69feb60ca6fba4ae0c8adeef6) 对报告内容进行排版；
        * `个人实践心得体会` 内容重点强调：个人在本次大作业中的主要贡献；完成了哪些自认为有技术含量的工作；印象深刻的一些 bug 和自己的解决方法；
    * 附件大小请控制在 ***10MB*** 以内，删除不必要的临时文件、视频文件、开发和测试过程中上传的测试文件等；
    * 视频文件可以上传到第三方视频网站，然后在总结报告文档中附上视频链接即可，以减少压缩包大小；
    * 已在 Github 上传所有文件的小组，在实验报告中同样需要附上项目仓库地址备查。
* **结课材料提交 DDL：2025.06.30 23:59:59** 。

### 推荐的实验报告目录组织形式

```
├── 0_张三 # 存放 `个人的实践心得体会`
│   └── README.md
├── 1_李四
│   └── README.md
├── 2_王五
│   └── README.md
├── 3_赵六
│   └── README.md
├── code  # 存放代码
├── docs  # 存放项目说明文档
└── README.md
```

- 如果是选择在 **公开仓库** 提交作品，则无需实名命名上述子目录，可以使用自己的 `网络 ID` ，但是在打包提交到畅课作业区的最终实验报告目录里需要替换为实名。

