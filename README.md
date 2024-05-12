# 数字集成电路设计ASIC流程
> 一个简单的项目，用于练习数字集成电路设计ASIC流程。

## 设计题目
基于已有设计 [ws2812 LED 灯带驱动](https://github.com/mattvenn/ws2812-core)，完成仿真验证、DC综合、形式验证、布局布线、后端版图验证、PT、后仿真验证等步骤。

## 文件结构
```
.
├── DC # DC 综合
│   ├── clean.sh
│   ├── Readme
│   ├── reports
│   ├── run_dc_constraint_compile.sh
│   ├── run_dc_read_rtl.sh
│   ├── scripts
│   ├── synopsys_dc.setup -> .synopsys_dc.setup
├── doc # 文档及报告的latex源码
│   └── pic
├── FM_RTL_PostDC # FM 形式验证
│   ├── clean.sh
│   ├── lib -> ../lib/
│   ├── netlist -> ../DC/netlist/
│   ├── Readme
│   ├── rtl -> ../rtl/
│   ├── run_fm.scr
│   ├── svf -> ../DC/svf/
│   ├── synopsys_fm.setup
│   └── ws2812.fms
├── lib # 工艺库
├── rtl # 设计的 verilog 源码
└── ws2812-core # ws2812 LED 灯带驱动仿真
```

## 备注
- 参照各个目录下的 `Readme` 文件，按照步骤进行设计。
- 根据实际情况，可能需要修改各个目录下的脚本文件，以适应自己的工程。

