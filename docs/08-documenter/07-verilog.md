---
description: Verilog/SV examples
---

# Verilog/SV examples

## Supported Labels
Here are the following labels supported by the documenter:
* Module Description
* Ports
* Parameters
* Constants
* Registers / Wires
* Always Block
* Instances
* Functions
* Typedefs

## Label Examples
### Module Description
#### Code
<code>// @title JeffModule</code> 

#### Result
![](/img/documenter/verilog/title.png)

#### Notes
Place at the top of the file

### Ports
#### Code
<code>input  clk, // input clock for module</code> 

#### Result
![](/img/documenter/verilog/port.png)
#### Notes
Comment needs to be inline with definition

### Parameters
#### Code
<code>parameter clk_freq_hz = 32'b0 //clock frequency</code>

#### Result
![](/img/documenter/verilog/parameter.png)   

#### Notes
Comment needs to be inline with definition

### Registers/Wires
#### Code
<code>reg [$clog2(1024)-1:0] count = 0; </code>

#### Result
![](/img/documenter/verilog/reg.png)  

#### Notes
Comment needs to be inline with definition

### Always Block
#### Code
<code>always @(posedge clk or negedge rstn) begin: my_counter</code>

#### Result
![](/img/documenter/verilog/always.png)  

#### Notes

### Instances

#### Code
#### Result
#### Notes


### Functions
#### Code
#### Result
#### Notes

### Typedefs
#### Code
#### Result
#### Notes