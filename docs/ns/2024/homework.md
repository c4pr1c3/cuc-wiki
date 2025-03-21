# 本学期课程考核规则

## 总成绩构成

等级成绩类型：百分制

总成绩 = `平时成绩` 系数*20% + `期末成绩` 系数*60% + `考勤成绩` 系数*10% + `线上成绩` 系数*10%

## 总成绩评定规则

* 详见 [在线成绩计算器](https://docs.qq.com/sheet/DVUxyT0VCcXdDZ2hE?tab=BB08J2) 中的示例数据和具体单元格的计算公式
    * 实验报告总分
    * 总分
* 实验报告要求继承上学期 《Linux 系统与网络管理》课程的实验报告要求

## 关于私有作业仓库的说明

由于在 `GitLab` 中，私有仓库不代表只有自己一个人可以访问，请看以下搬运自 `GitLab` 创建新仓库时关于 `Private` 属性的说明文字：

> Project access must be granted explicitly to each user. If this project is part of a group, access is granted to members of the group.

翻译如下：

> 必须向每个用户显式授予项目访问权限。如果此项目是用户组的一部分，则向组成员授予访问权限。

据此可以更好地理解在 `GitLab` 中，在一个用户组命名空间下创建的 `私有仓库`，对于组内的所有用户来说，实际上是相互可见、内部公开的。

以下作业要求里提到的 `私有作业仓库` 具体指的是： **仅限仓库创建者本人、四名助教、任课老师** 有权限访问该仓库，其他同学即使知道该仓库链接地址也无法访问仓库内容。

具体操作步骤建议如下：

- 在自己个人命名空间下创建仓库。此处假设个人用户名是 `zhangsan` ，创建的私有仓库名为 `ns-private` 。
- 在自己个人命名空间下创建的仓库里，通过左侧导航菜单的 `Project information` - `Members` 进入仓库用户管理页面，点击右上角的 `Invite members` ，通过输入实名的方式，搜索、选中搜索结果，邀请 4名助教、任课老师，授予 `Maintainer` 角色。
- 在自己的组命名空间下（当前为 `ccs/ns-2024` ）的组内公开仓库根目录下的 `README.md` 添加指向上述私有仓库的超链接：`zhangsan/ns-private`。

## 平时成绩

1. `平时成绩` 满分按照 100 分计算。
2. `平时成绩` 重点关注同学们的 `学习态度` 和 `课堂表现` 等综合评价。
3. `学习态度`：同学们在畅课平台上的 `讨论区` 发帖数量和质量的综合评价。“发帖”数量统计包括“新发帖”数量、“回复发帖”数量。质量评价是基于客观事实的主观评价，评价标准主要包括帖子内容与课程内容的相关性、帖子内容的原创性、帖子内容的排版质量、帖子内容对其他同学的有效帮助或启发（点赞数量会作为辅助评价指标）等。`学习态度` 及格标准为 1 条有效“发帖”，满分标准为 5 条有效“发帖”或 1 条高质量“发帖”。
4. `课堂表现`：本学期的所有课堂实验环节都将给同学们提供“翻转课堂”的机会。通过课堂上随机点名的方式，挑选同学上讲台进行 5~10 分钟的专题知识点、技能点分享。分享后还需要接受现场老师和台下同学们的提问，由老师根据同学们的分享内容质量和回答问题质量进行综合评价。每个同学在一学期内最多有 2 次分享机会，取最高成绩计入平时成绩。
5. `平时成绩` = `max(学习态度, 课堂表现)`。

## 期末成绩

0. 所有实验报告得分之和构成期末成绩。
1. 实验报告题目一：第一章、第五章、第十一章课后实验报告。
2. 实验报告题目二：第八章、第九章和第十二章课后实验报告至少任选其一。
3. 实验报告题目一得分占比 80%，实验报告题目二得分占比 20%。
4. 需要提交到 **私有作业仓库** 的实验报告是：第十一章。
5. 没有特别说明的实验报告默认提交到公开仓库。

## 考勤成绩

* 线下课一共 16 次，每次正常考勤记 5 分，全勤加 20 分。
* 迟到半小时以内记考勤 4 分。
* 早退或迟到超过半小时后，每满 10 分钟或不足 10 分钟，均扣考勤 1 分。如此累进扣分，扣到 0 分为止。
* 缺勤记 0 分。
* 正常规范请假按正常考勤记录，需提前 24 小时请假。其他情况酌情扣分。
* 如因不可抗力因素导致线下课总次数不等于 16 次，则临时微调考勤成绩计算方法。

## 线上成绩

* 畅课平台上单元测试成绩之和，按满分 100 分进行等比例折算。

