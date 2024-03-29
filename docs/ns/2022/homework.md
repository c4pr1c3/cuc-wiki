# 本学期课程考核规则

## 总成绩构成

等级成绩类型：百分制

总成绩 = `平时成绩` 系数*20% + `期末成绩` 系数*60% + `考勤成绩` 系数*10% + `线上成绩` 系数*10%

## 总成绩评定规则

* 详见 [在线成绩计算器](https://docs.qq.com/sheet/DVUVMalZWRnFZd0lQ?tab=BB08J2) 中的示例数据和具体单元格的计算公式
    * 实验报告总分
    * 总分
* 实验报告要求继承上学期 《Linux 系统与网络管理》课程的实验报告要求

## 平时成绩

1. `平时成绩` 满分按照 100 分计算。
2. 自行选择 `在线 CTF 平台` 完成 `刷题百分` 打卡，并撰写配套 `CTF WriteUp`。
3. `平时成绩` 计算截止时间为考试周前一天晚上 23:59:59 。
4. 所有 `CTF WriteUp` 提交到 **私有作业仓库** 独立目录下，每道得分题均需配套 `WriteUp`；缺少配套 `WriteUp` 则对应题目得分可能被视为无效。

### 在线 CTF 平台

`刷题百分` 推荐平台如下，推荐优先级从高到低排列：

- [CTFHub](https://www.ctfhub.com/)
- [BUUCTF](https://buuoj.cn/)
- [XCTF](https://adworld.xctf.org.cn/challenges/list)

学习和体验用途，不参与 `刷题百分` 的平台推荐如下：

- [Bugku](https://ctf.bugku.com/)
- [hackthebox](https://www.hackthebox.com/)

### 刷题百分

| 难度级别   | 分值 | CTFHub    | BUUCTF                  | XCTF      | 
| :-         | :-   | :-        | :-                      | :-        | 
| ⭐️         | 5    | 2星及以下 | >=2000次解出            | 2星及以下 | 
| ⭐️⭐️       | 10   | 3星       | [1000,2000)次解出       | 3星       | 
| ⭐️⭐️⭐️     | 15   | 4-5星     | [100,1000)次解出        | 4-5星     | 
| ⭐️⭐️⭐️⭐️   | 20   | 6-8星     | 小于100次解出且小于90分 | 6-8星     | 
| ⭐️⭐️⭐️⭐️⭐️ | 50   | 9-10星    | >=90分                  | 9-10星    | 

补充说明：

- 由于这些平台的开放性和已解题人员数量、难度评分的动态性，需要出具包含上述 `证明信息` 和带有 [时间戳](https://www.baidu.com/s?ie=utf-8&wd=%E7%8E%B0%E5%9C%A8%E6%97%B6%E9%97%B4) 的做题时截图。
- 难度级别请对照上述难度级别说明自评，并在 `WriteUp` 里汇总一个「目录清单」，每道题目的 `WriteUp` 显著位置标注上难度级别。
- 如发现 `PS 截图造假` 或 `难度级别自评错误`，则取消对应题目 `WriteUp` 的计分。
- 所谓 `刷题百分` 就是提交的 `WriteUp` 包含的题目总分值达到或超过 `100` 分，此时 `平时成绩` 得分为满分。
- 最终认定的 `刷题百分` 总分值如果不满 `100` 分，则按照实际得分计入平时成绩。
- `WriteUp` 中需要包含 `证明自己亲自动手完成实验的「特征标志」`。例如，使用的 `Linux` 终端提示符里包含自己姓名拼音或简拼或自己的 `Github ID` 等。需要注意的是，后期图片处理加上的 `水印` 没有亲自动手完成实验的证明力。
- 无上述 `证明自己亲自动手完成实验的「特征标志」` 的题目对应 `WriteUp` 不予计分。

举例说明：

- `张三` 在 `CTFHub` 平台上完成了 10 道 `⭐️` 难度题目的 `WriteUp`、2 道 `⭐️⭐️` 难度题目的 `WriteUp`、3 道 `⭐️⭐️⭐️` 难度题目的 `WriteUp` ，则总分达到 115 分，平时成绩满分。
- `李四` 在 `CTFHub` 平台上完成了 5 道 `⭐️` 难度题目的 `WriteUp`、2 道 `⭐️⭐️` 难度题目的 `WriteUp`、3 道 `⭐️⭐️⭐️` 难度题目的 `WriteUp` ，则总分达到 90 分，平时成绩 90 分。

## 期末成绩

0. 所有实验报告得分之和构成期末成绩。
1. 实验报告题目一：第一章、第五章、第七章、第十一章课后实验报告。
2. 实验报告题目二：第二章、第三章、第四章、第八章、第九章、第十章和第十二章课后实验报告至少任选其二。
3. 实验报告题目一得分占比 80%，实验报告题目二得分占比 20%。
4. 需要提交到 **私有仓库** 的实验报告是：第七章和第十一章。
5. 没有特别说明的实验报告默认提交到公开仓库。

## 考勤成绩

* 线下课预计一共 9 次，每次正常考勤记 10 分，全勤加 10 分。
* 迟到半小时以内记考勤 8 分。
* 早退每满 10 分钟或不足 10 分钟，均扣考勤 1 分。扣到 0 分为止。
* 缺勤记 0 分。
* 如果因不可抗力因素导致线下课总次数不等于 9 次，则临时微调考勤成绩计算方法。

## 线上成绩

* 畅课平台上单元测试成绩之和，按满分 100 分进行等比例折算。

