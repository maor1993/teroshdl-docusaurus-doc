---
description: usage of state machine 
---

# Introduction
TerosHDL attempts to recognize any state machines used in the Verilog/VHDL code.

Included is a built in visualizer which allows you to view previously detected state machines.

## Usage
While having an HDL file open, you can click on the state machine viewer on the top right of the editor:

<p align="center">
<i>Image 1: State Machine Viewer Button </i>

![State Machine Viewer Button](/img/state_machine_viewer/sm-button.png) 
</p>

This will pop up a new window with all of the state machines found in this file:

<p align="center">
<i>Image 1: State Machine Window </i>

![State Machine Window](/img/state_machine_viewer/sm-window.png) 
</p>


When you click on one of the state arrows, or the state themselves; TerosHDL will highlight the corresponding code area which causes this change.


:::tip
Any State machines that we're detected will also be added to the documentation of the file
:::



