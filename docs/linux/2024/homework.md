# 本学期课程考核规则

## 总成绩构成

等级成绩类型：百分制

总成绩 = `平时成绩` 系数*30% + `期末成绩` 系数*60% + `线上成绩` 系数*10%

## 总成绩评定规则

* 详见 [在线成绩计算器](https://docs.qq.com/sheet/DVU1aRFRJSlNQSmNV?tab=BB08J3) 中的示例数据和具体单元格的计算公式。
    * 如果需要通过编辑文档来自行“预估”自己的期末成绩，你可以登录腾讯文档后，复制当前共享表格到你自己的账号里。 **不需要向我申请文档编辑权限，不会同意的。**

## 平时成绩

* 基于 `客观事实` 的「主观评价」。`客观事实` 来源包括但不限于：在校内畅课平台上的讨论区提出好问题、回答问题对其他同学产生了有效帮助、课堂上积极参与互动、畅课学习完成度、`课程公共服务器` 的使用次数和时长等。 ** 数据统计截止本学期最后一次课程结束 `2024.6.19 09:50:00` ** 。
* 满分 30 分的平时成绩中，有 10 分来自于 `考勤成绩` 。`考勤成绩` 计算规则见以下小节详细说明。

### 考勤成绩

* 本学期一共记录考勤 8 次，每次正常签到得 1 分，迟到得 0.5 分，旷课得 0 分。有假条的病事假按正常签到计分。
* 学期考勤全勤（累计计分 8 分），获得全勤加分 2 分。
* 学期考勤累计计分 [6, 8)，获得考勤加分 1 分。
* 学期考勤累计计分 [5, 6)，无考勤加分。
* **学期考勤累计计分 [0, 5)，直接挂科** 。

## 期末成绩

* 8 章课程，每章课后均留有作业，按章节顺序分别记为：H1 ~ H8
  * 满分 10 分的 **必选** 作业：H1, H2, H3 。
  * 满分 20 分的 **必选** 作业：H4 。
  * 满分 10 分的 **四选一** 作业：H5, H6, H7, H8。该项计分公式为：max(H5, H6, H7, H8) 。
  * H1, H2, H3 作业采用 `基于日志分析的自动判题方式` ，不需要撰写实验报告，但需要访问课程指定的 Linux 远程云主机并自行独立完成相应的实验任务。
  * H4 作业采用 `Gitlab CI/CD` 方式，不需要撰写实验报告。
  * **四选一** 作业需要提交实验报告。
* **H6, H7, H8 要求提交到私有仓库，其他章节作业均提交到公开仓库**。
* [每次实验报告的评分标准见教学 Wiki 首页说明 - 缺省的实验报告评分标准](../../index.md#_5)
* 请仔细阅读 [关于 GitLab 使用的规范和要求](gitlab.md) ，按照规范使用对应的公开和私有作业仓库。
* 以上作业完成时间截止时间为本学期最后一次课程结束后一周： `2024.6.26 23:59:59` 。

### 关于私有作业仓库的说明

由于在 `GitLab` 中，私有仓库不代表只有自己一个人可以访问，请看以下搬运自 `GitLab` 创建新仓库时关于 `Private` 属性的说明文字：

> Project access must be granted explicitly to each user. If this project is part of a group, access is granted to members of the group.

翻译如下：

> 必须向每个用户显式授予项目访问权限。如果此项目是用户组的一部分，则向组成员授予访问权限。

据此可以更好地理解在 `GitLab` 中，在一个用户组命名空间下创建的 `私有仓库`，对于组内的所有用户来说，实际上是相互可见、内部公开的。

以下作业要求里提到的 `私有作业仓库` 具体指的是： **仅限仓库创建者本人、1名助教、任课老师** 有权限访问该仓库，其他同学即使知道该仓库链接地址也无法访问仓库内容。

具体操作步骤建议如下：

- 在自己个人命名空间下创建仓库。此处假设个人用户名是 `zhangsan` ，创建的私有仓库名为 `linux-private` 。
- 在自己个人命名空间下创建的仓库里，通过左侧导航菜单的 `Project information` - `Members` 进入仓库用户管理页面，点击右上角的 `Invite members` ，通过输入实名的方式，搜索、选中搜索结果，邀请 4名助教、任课老师，授予 `Maintainer` 角色。
- 在自己的组命名空间下（当前为 `ccs/linux-2024` ）的组内公开仓库根目录下的 `README.md` 添加指向上述私有仓库的超链接：`zhangsan/linux-private`。

## 线上成绩

* 校内畅课平台上单元测试成绩累加后进行等比例折算。
