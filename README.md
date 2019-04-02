# 华中科技大学计算机学院 Verilog 语言课程
这个项目是为华中科技大学计算机学院的 “Verilog 语言” 课程准备的，涵盖了课程须知、实验指南、以及所需要的其它材料。
## 课程目标
- 通过课程的学习，掌握 Verilog HDL 硬件描述语言的语法知识和程序结构
- 掌握应用 Xilinx Vivado 进行 Verilog 程序设计和开发的基本流程和方法
- 建立 Verilog 硬件设计的基本概念，会使用 Verilog 语言描述、设计简单的数字电路
## 教材及参考书籍
- 教材：Verilog HDL 入门，第3版（A Verilog HDL Primer, Third Edition），（美）巴斯克著，夏宇闻、甘伟译，北京航空航天大学出版社，2008.
- 参考书：EDA 技术实用教程 ———— Verilog 版（第五版），潘松、黄继业，科学出版社，2010.
- 以上书籍“京东”、“亚马逊”有售。
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
- 若希望在自己的 PC/Mac 上安装 Vivado，可以在 Xilinx 网站下载安装该版本。新版 Vivado，使用界面与实验室略有不同，适合有兴趣的同学自行摸索。
- Vivado for Windows 版适用于 Windows 7 / Windows 10。（[百度下载](https://pan.baidu.com/s/15eftbUP_h7w1AGIHujHKFQ)，提取码: j682）
### 实验指导书
- [实验指导书下载](./实验指导书/实验指导书.v1.0.rar)
