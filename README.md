# 编译原理实验安排

最新实验内容和通知请参考网址: https://github.com/comp1ler/Compiler2020

> 2020年12月7日：实验三截止，公布实验四要求及截止日期

> 2020年11月14日：实验二截止，公布实验三要求及截止日期

> 2020年10月19日：实验一截止，公布实验二要求及截止日期

> 2020年9月30日：公布分组名单，并更新实验一选做要求

> 2020年9月28日：发布实验一及分组截止日期

---

如遇到问题请*联系助教*

助教邮箱
- yuli@smail.nju.edu.cn


## 1. 基本内容

编译原理的实验内容是实现一个类C语言(C--)的编译器: 将C--源代码转换成标准的MIPS汇编代码的编译器，所得到的汇编代码可以在SPIM Simulator上运行。

实验安排中有4次实验，**具体要求见对应链接**：
- [实验一: 词法和语法分析](Lab1.md)
- [实验二: 语义分析](Lab2.md)
- [实验三: 中间代码生成](Lab3.md)
- [实验四: 目标代码生成](Lab4.md)

实验教材为: *《编译原理实践与指导教程》，许畅 陈嘉 朱晓瑞编著*

## 2. 评分标准


> 实验最终得分为: 实验得分 * 得分系数 - 扣分项

关于实验最终得分有以下说明：

- 实验得分会综合考虑用例通过情况、实验报告、代码实现情况等，不会难为大家😀
- 实验得分系数分别为 1.1(1人组队), 1.0(2人组队), 0.9(3人组队)
- 扣分项主要是一些违反提交、运行要求的行为


## 3. 实验提交要求

1. 每次实验在截止日期之前提交到助教邮箱: yuli@smail.nju.edu.cn
2. 每次实验提交内容只包含一个压缩包文件: 组长学号_姓名_LabX_vY_groupZ.zip, 邮件标题为 "Compiler2020-LabX", 其中X表示第几次实验, Y表示第几次版本, Z表示分组号码, 使用具体信息替换 XYZ(如"18122xxxx_张三_Lab1_v1_group5.zip")
3. 压缩包内容如 Lab.zip 所示, 包含源程序, 可执行文件, 实验报告(2-3页), 提交时注意文件名命名
4. 使用给定 Makefile 进行编译, 自己另外构造的 Makefile 无效
5. 每次实验提交内容按要求进行提交, 违反者会进行倒扣分


## 4.测试环境

实验验收的测试环境如下：

1. GNU Linux Release: Linux Mint 19.2, kernel version 4.15.0;
2. GCC version 7.4.0;
3. GNU Flex version 2.6.4;
4. GNU Bison version 3.0.4。

测试环境仅供参考，实验的指导用书中也有关于实验环境配置的内容，可以自行查阅。

> 一般而言，只要避免使用过于冷门的特性，使用其它版本的Linux或者GCC等，也基本上不会出现兼容性方面的问题。

另外有一些可能会对你有帮助的注意点：

- wsl应该也可以，不过实验第三阶段会用到qt实现的gui应用，可能需要额外的配置
- Ubuntu 20.04把pyqt4从官方的软件源里去掉了，所以在第三阶段使用gui应用时也需要另外的处置
