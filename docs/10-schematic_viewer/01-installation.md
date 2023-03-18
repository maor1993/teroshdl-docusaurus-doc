---
description: setup of schematic viewer
---

# Installation

## Preface
TerosHDL supports a basic visualization of the current file you have open.

TerosHDL uses [yosys](https://github.com/YosysHQ/yosys), which is an open source hdl synth tool.

the following section describes how to get your environment ready for using the schematic viewer


## Installation
### Verilog
If you plan to only use verilog in your designs, you can use yowasp-yosys, which is a distribution of yosys running as an executable.

you only need to run the following command:
```
pip install teroshdl
```
this will install the necessary additional packages for TerosHDL.
to use yowasp-yosys, select **YOWASP** in the configuration menu.


### VHDL
Yosys was natively designed to work with verilog and thus an additional plugin is required to support VHDL.

TerosHDL suggests you use oss-cad-suite, which is a prebuilt collection of tools which also includes yosys + vhdl support.
you can download oss-cad-suite by following this [link](https://github.com/YosysHQ/oss-cad-suite-build/releases)

:::note
TerosHDL expects the tools to be available in the PATH variable, ensure you add the "bin" folder of the oss-cad-suite to your operating system PATH variable.
:::

To use yosys+ghdl, select **Yosys + GHDL(module)** in the configuration menu.

