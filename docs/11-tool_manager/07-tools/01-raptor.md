---
description: Raptor
---

# Raptor

## Configuration

1. Configure your Raptor binary directory in the [TerosHDL configuration](../../02-getting_started/03-views.md#configuration-menu): `TerosHDL configruation >> Tools >> Raptor Design Suite >> Installation path`. E.g: `/opt/RapidSilicon/Raptor/2023.04/bin`
2. Select Raptor as your tool: `TerosHDL configuration >> Tools >> General >> Tool`.

## New project creation

:::caution

Don't add the testbenches as source. You need to configure your testbench in the Raptor configuration menu.

:::

1. [Create an empty project](../02-project.md#adding-a-project)
2. [Add your sources](../03-source.md#adding-source)
3. [Select your toplevel file](../03-source.md#setting-project-toplevel-file)

## Bitstream generation

1. [Run the bitstream generation](../04-run.md#running-your-tool). You will see the message "TerosHDL: tool running" in the left bottom corner.
2. Check the output log in the `TerosHDL: Tool manager` console.

<p align="center">

![Run view](/img/tool_manager/tools/raptor/console.png) 
</p>

3. [Check the artifacts](../05-output.md): 
    - Summary: TCL project file.
    - Routing, Place... reports.
    - Simulation waveforms.

## Running a simulation

1. Configure your GTKwave binary path: `TerosHDL configuration >> Tools >> General >> GTKWave installation directory`.
2. In the Raptor configuration (`TerosHDL configruation >> Tools >> Raptor Design Suite`) select `RTL simulation`, `Simulate Gate`...
3. Create a new project.
4. Add your desing sources and constraints files.
5. Configure your top testbench path in: `TerosHDL configruation >> Tools >> Raptor Design Suite >> Simulation top level path`. E.g: `/home/carlos/rapidsilicon/tcl_examples/counter_vhdl/testbench.vhd`.
6. Configure other testbench sources in: `TerosHDL configruation >> Tools >> Raptor Design Suite >> Other simulation sources`. E.g: `/home/carlos/rapidsilicon/tcl_examples/counter_vhdl/testbench.vhd, /home/carlos/rapidsilicon/tcl_examples/counter_vhdl/other_testbench.vhd`. If you want to add more than one source you need to put a comma: `/source/one.v, /source/two.v`
7. [Run Raptor](../04-run.md#running-your-tool)
8. Open your waveform from the output view.


## Running a Raptor project sample

You can add a Raptor project sample from [the TerosHDL menu](../02-project.md#adding-a-project):

- raptor_counter
- raptor_counter_vhdl
- AES_DECRYPT
- raptor_and2_gemini

## Cleaning your project stages

<p align="center">

![Run view](/img/tool_manager/tools/raptor/clean.png) 
</p>

