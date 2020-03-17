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
  + [Vivado Lab 2019.2 for Windows](#Vivado-Lab-20192-for-Windows)
- [Q&A](#QA)
  + [Q：连不上实验板怎么办？](#Q连不上实验板怎么办)
  + [Q：安装完毕后，仿真（Simulation）、综合（Synthesis）、实现（Implementation）等功能不能正常运行怎么办？](#Q：安装完毕后，仿真（Simulation）、综合（Synthesis）、实现（Implementation）等功能不能正常运行怎么办？)



## 课程目标

- 通过课程的学习，掌握 Verilog HDL 硬件描述语言的语法知识和程序结构
- 掌握应用 Xilinx Vivado 进行 Verilog 程序设计和开发的基本流程和方法
- 建立 Verilog 硬件设计的基本概念，会使用 Verilog 语言描述、设计简单的数字电路



## 教材、参考书籍

- 教材：Verilog HDL 入门，第3版（[PDF](./manual/a-verilog-hdl-primer.pdf)），（美）巴斯克著，夏宇闻、甘伟译，北京航空航天大学出版社，2008.
- 参考书：EDA 技术实用教程 — Verilog 版（第五版），潘松、黄继业，科学出版社，2010.



## 课件

[课件（含讲解）百度下载](https://pan.baidu.com/s/1QsUyEVH8zHAkgsxb3p1x_A)，提取码: cyi3。

[课件下载（Github）](./lecture)



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

- 实验室软件环境为：Xilinx Vivado HLx Editions 2015.2（并非 Vivado 的最新版本）。
- 若希望在自己的 PC 上安装 Vivado，可以在 Xilinx 网站下载安装该版本。
  - Vivado 只支持 Windows / Linux，并不支持 macOS。
- 最新版 Vivado 兼容本课程的所有实验，其使用界面与 2015.2 略有不同，适合有兴趣的同学自行摸索。
- 可以使用（[Vivado 百度下载](https://pan.baidu.com/s/1ZoIvpsieQuQ3IRlmIStG9A)，提取码: xdnn）来加速下载。
- 2020-03-13 更新：百度下载添加 Vivado HLx Editions 2019.2 版本下载。
- 2020-03-13 更新：百度下载添加 Vitis Core Development Kit 2019.2 版本下载。

### 实验指导书

- [实验指导书下载](./instruction/experiment-instruction.v1.rar)

### Vivado HLx Editions 和 Vitis Core Development Kit

Xilinx 在 2019 年 10 月，推出了 “Vitis” 统一软件平台，其包括目标平台、核心开发套件、加速库和特定领域开发环境，能够让软硬件开发者们在无需掌握硬件专业知识的情况下，根据软件或算法代码来自动适配并使用赛灵思的硬件架构。

实际上，Vitis 可以视为：C/C++/Python 开发工具 + Vivado 硬件开发工具 + AI 加速库 + 其它加速库。它可以让软件开发人员在无需掌握硬件专业知识的情况下，利用加速库来使用 FPGA 进行硬件加速；也让硬件开发人员设计的硬件快速嵌入到软件平台。

同时，Xilinx 面向硬件开发人员也提供独立的 Vivado HLx Edition。

目前（2020-03-13），Vitis 的最新版本是 Vitis Core Development Kit 2019.2 Update 1；Vivado 的最新版本是 Vivado HLx Edtions 2019.2 Update 1。

### License

- 请安装 Vivado Webpack 版本，因为：
  - Webpack 版本在功能上没有缺失。
  - 相比 HLx 版本，Webpack 版支持的器件较少。
  - Webpack 版本完全免费。
  - Webpack 版本完全满足课程学习的要求。
- Vivado 和 Vitis ，安装 Webpack 版本的方法略有不同。
  - Vivado（2015.2 / 2019.2）在安装时，需选择安装 Webpack 版本。请参考 [“简明安装指南”](./install-guide.md)。
  - Vivado 2015.2 版需在 [Xilinx License](http://www.xilinx.com/getlicenses) 申请 Webpack License（免费），并安装在自己的 PC 上。
  - Vivado 2019.2 版 License：当设计中只使用了 Webpack 所支持的器件时（包括我们实验所用的 A7 系列 FPGA），Vivado 将跳过 License 检查，因此无需申请 License，也没有任何物理的 License 文件。
  - Vitis 安装过程中没有 Webpack 选项，但是它执行和 Vivado 2019.2 版本一样的 License 策略，即：无需任何的 License 就可以完成课程实验。
- 建议安装 Vivado 2019.2 Webpack 版来完成课程实验。



## Q&A

### Q：连不上实验板怎么办？

连不上实验板有以下几种可能性：

**1. Xilinx USB Cable Driver 挂死。**

  原因：由于没有按照正确的顺序插拔、开关实验板，可能导致 Xilinx USB Cable Driver 挂死。

  解决方案：

  - 关闭实验板电源，将实验板从 USB 口拔下。
  - 重新启动 PC。
  - 将实验板插上，打开实验板电源开关。
  - 如还不能正确连接，尝试换一个 USB 接口。

**2. 没有正确安装 Xilinx USB Cable Driver。**

  原因：在 Vivado 安装时，没有选中“安装 Xilinx USB Cable Driver”，或没有按照要求：在安装过程中拔下实验板。

  解决方案：

  - 关闭实验板电源，将实验板从 USB 口拔下。
  - 重新启动 PC。
  - 单独安装 Xilinx USB Cable Driver，安装过程参考官方文档：
      - [“在不全面重新安装 Vivado 设计套件的情况下，是否能够（重新安装）安装 Xilinx USB/Digilent 线缆驱动器？(中文）”](https://china.xilinx.com/support/answers/59128.html)
      - 或 [ "Is it possible to (re)install the Xilinx USB/Digilent cable drivers without a full reinstall of Vivado Design Suite? (English)"](https://www.xilinx.com/support/answers/59128.html)。

  ### Q：安装完毕后，仿真（Simulation）、综合（Synthesis）、实现（Implementation）等功能不能正常运行怎么办？

  **1. 检查 Vivado 版本和 License**

  如果安装的是 Webpack 版，是不需要 License 的；如果安装的是 Design Edition 或 System Edition，则需要 License。建议安装 Webpack 版本。

  **2. 防病毒软件可能会导致安装不正确**

  360、腾讯电脑管家可能会阻止某些 .bat 文件的运行，阻止修改系统设置，从而导致 Vivado 安装不正确。建议：关闭防病毒软件后，重新安装 Vivado；在运行 Vivado 时，保持防病毒软件关闭。

