## Yosys
```bash
yosys											启动
```
## Parsing
```bash
read_verilog <filename>							Load modules from a Verilog file

```
## Elaboration
```bash
hierarchy -check -top <module>					check the design hierarchy,specify top module
dump											print parts of the design in RTLIL format
write_rtlil [filename] 							write design to RTLIL file
show											generate schematics using graphviz
proc 											translate processes to Word-level cells
```
## Coarse-grain synthesis
```bash
opt 											optimizations
fsm												extract and optimize finite state machines
memory											translate memories to basic cells

```
## Fine-grain synthesis
```bash
techmap											translate Word-level to Gate-level
splitnets -ports								splits multi-bit nets into single-bit nets
opt -full										

```
## Technology mapping
```bash
dfflibmap -liberty <xxx.lib>					technology mapping of flip-flops
read_liberty -lib <xxx.lib>						使 show 显示正确
abc -liberty <xxx.lib>							technology mapping to logic

```
## Synthesis output
```bash
write_verilog netlist.v 						write design to Verilog file
stat -liberty <xxx.lib> 						print some statistics
```