# Vivado HLx 2018.3 安装指南

## 操作系统

**Xilinx 强烈建议大家检查操作系统的版本号！**

由于 Vivado 是一个专业软件，和 Office 等大众软件不同，Xilinx 公司并没有在所有的环境下测试软件的兼容性。很多运行问题，均是由于操作系统兼容性引起的。例如：在进行仿真时，出现无法仿真，log 文件显示：“ERROR: [XSIM 43-3410] Failed to compile one of the generated C files.” 错误。[Xilinx 对该问题的官方解决方案](https://forums.xilinx.com/t5/Simulation-and-Verification/ERROR-XSIM-43-3410-Failed-to-compile-one-of-the-generated-C/td-p/713272) 就指出：操作系统版本不正确，可能会导致该问题。

Vivado HLx 2018.3 要求的操作系统版本如下：
- Windows 7.1: 64-bit
- Windows 10 Professional version 1803 and 1809: 64-bit
- Red Hat Enterprise Linux 6.6-6.9: 64-bit
- Red Hat Enterprise Linux 7.2-7.5: 64-bit
- CentOS Linux 6.6-6.9: 64-bit
- CentOS Linux 7.2-7.5: 64-bit
- SUSE Enterprise Linux 11.4: 64-bit
- SUSE Enterprise Linux 12.3: 64-bit
- Ubuntu Linux 16.04.4 and 18.04 LTS: 64-bit - Additional library installation required

Vivado 2018.3 需要 Windows 10 Professional 1803 and 1809 x64 版本。非专业版，或子版本号低于 1803 的，可能会出现未知的问题。
