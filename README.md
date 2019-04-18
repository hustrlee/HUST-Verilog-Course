# 华中科技大学计算机学院 Verilog 语言课程

这个项目是为华中科技大学计算机学院的 “Verilog 语言” 课程准备的，涵盖了课程须知、实验指南、以及所需要的其它材料。

## 目录

- [课程目标](#课程目标)
- [教材、参考书籍](#教材参考书籍)
- [课件](#课件)
- [实验须知](#实验须知)
  + [硬件环境](#硬件环境)
  + [软件环境](#软件环境)
  + [实验指导书](#实验指导书)
  + [Vivado HLx 2018.3](#Vivado-HLx-20183)
- [Q&A](#QA)
  + [Q：连不上实验板怎么办？](#Q连不上实验板怎么办)

## 课程目标

- 通过课程的学习，掌握 Verilog HDL 硬件描述语言的语法知识和程序结构
- 掌握应用 Xilinx Vivado 进行 Verilog 程序设计和开发的基本流程和方法
- 建立 Verilog 硬件设计的基本概念，会使用 Verilog 语言描述、设计简单的数字电路

## 教材、参考书籍

- 教材：Verilog HDL 入门，第3版（A Verilog HDL Primer, Third Edition），（美）巴斯克著，夏宇闻、甘伟译，北京航空航天大学出版社，2008.
- 参考书：EDA 技术实用教程 ———— Verilog 版（第五版），潘松、黄继业，科学出版社，2010.
- 以上书籍“京东”、“亚马逊”有售。

## 课件

[课件下载](./PPT/)

## 教学安排

| 课次 | 授课类别 | 教学内容 | 课时 |
|:----:|:-------:|---------|------|
| 1 | 理论讲授 | - Verilog HDL 语言简介<br>- Verilog HDL 语言基础 | 4 学时 |
| 2 | 实验 | - Vivado 的使用及设计流程 | 4 学时 |
| 3 | 理论讲授 | - Verilog HDL 程序设计方法 | 4 学时 |
| 4 | 实验 | - 简单组合电路设计 | 4 学时 |
| 5 | 实验 | - 简单时序电路设计 | 4 学时 |
| 6 | 理论讲授 | - 简单数字电路设计 | 4 学时 |
| 7 | 实验 | - 数据通路设计 | 4 学时 |
| 8 | 实验 | - 有限状态机（FSM）设计 | 4 学时 |

## 实验须知

- **注意：课堂实验时间较短，请大家事先预习，才能更好地在课堂上完成实验**

### 硬件环境

- 实验需用到 DIGILENT 公司的 Nexys4 FPGA Board，请各班班长、学委于实验课前，按到课人数，向实验室统一借取实验板；并于实验结束后，统一归还。
- 实验板有两种，Nexys4 和 Nexy4 DDR。两种实验板的约束文件不同，请大家注意领取的实验板型号（在盒子封面以及实验板的中心位置有标识），使用不同的约束文件。（[Nexys4 约束文件](./Nexys4/Nexys4_Master.xdc)、[Nexys4 手册](./Nexys4/Nexys4_RM_VB2_Final_5.pdf)、[Nexys4 DDR 约束文件](./Nexys4/Nexys4DDR_Master.xdc)、[Nexys4 DDR 手册](./Nexys4/nexys4ddr_rm.pdf)）

### 软件环境

- 实验软件环境为：Xilinx Vivado 2015.2（并非 Vivado 的最新版本）。
- 若希望在自己的 PC/Mac 上安装 Vivado，可以在 Xilinx 网站下载安装该版本。
- 最新版 Vivado 也可以兼容本课程的所有实验，其使用界面与 2015.2 略有不同，适合有兴趣的同学自行摸索。
- 可以使用（[Vivado 百度下载](https://pan.baidu.com/s/15eftbUP_h7w1AGIHujHKFQ)，提取码: j682）来加速下载。
- 4/9/2019 更新：百度下载添加 Vivado 2018.3 版本下载。

### 实验指导书

- [实验指导书下载](./实验指导书/实验指导书.v1.0.rar)

### Vivado HLx 2018.3

目前（4/9/2019），Vivado 的最新版本是 Vivado HLx 2018.3 Update 1。其安装程序由：Vivado HLx 2018.3 和补丁包 Update 1 构成。完整安装需先安装 Vivado HLx 2018.3，再安装 Update 1。由于 Update 1 只是添加了对更多 device 的支持，对于本课程来说并不需要，因此无需安装 Update 1，仅安装 Vivado HLx 2018.3 本体即可。

Vivado HLx 2018.3 相较于 Vivado 2015.2 稳定性有较大提高，已经可以很好的处理 Unicode 的问题，对中文的支持较完善，不再要求全英文路径；同时，界面风格也更现代化。建议升级到 Vivado HLx 2018.3 来学习本课程。

Vivado 是一个专业软件，相较于 Office 等大众软件来说，安装选项比较复杂，如开发环境不能正常运行，请参考[“Vivado HLx 2018.3 安装指南”](./install_guide.md)。

## Q&A

### Q：连不上实验板怎么办？

连不上实验板有以下几种可能性：

1. Xilinx USB Cable Driver 挂死。
  
  原因：由于没有按照正确的顺序插拔、开关实验板，可能导致 Xilinx USB Cable Driver 挂死。
  
  解决方案：
  
  - 关闭实验板，并将实验板从 USB 口拔下。
  - 重新启动 PC。
  - 将实验板插上，并打开电源开关。
  - 如还不能正确连接，尝试换一个 USB 接口。
  
2. 没有正确安装 Xilinx USB Cable Driver。

  原因：在 Vivado 安装时，没有选中“安装 Xilinx USB Cable Driver”，或没有按照要求：在安装过程中，应拔下实验板。
  
  解决方案：
  
  - 关闭实验板，并将实验板从 USB 口拔下。
  - 重新启动 PC。
  - 单独安装 Xilinx USB Cable Driver，安装过程参考官方文档：[“在不全面重新安装 Vivado 设计套件的情况下，是否能够（重新安装）安装 Xilinx USB/Digilent 线缆驱动器？(中文）”](https://china.xilinx.com/support/answers/59128.html)，或[ "Is it possible to (re)install the Xilinx USB/Digilent cable drivers without a full reinstall of Vivado Design Suite? (English)"](https://www.xilinx.com/support/answers/59128.html)。
