## Verilator
```yaml
-cc:									C++ output mode
--exe:									Generate an executable,Default is a library
--trace-vcd:							Enable VCD
-f:										Parse arguments from a file

```

## veripool.org
```yaml
structure-of-the-verilated-model:		模块 port 和 reg 和 wire 访问方式	
DPI-C:									
```
## Language Extensions
```text
/*verilator public*/:
	1. (on typedef enum)				暴露.V/.SV 枚举类型,在 C++ 中可使用它
	2. (on variable)					
	3. 

/*verilator public_flat*/				
	1. (on variable)					暴露信号,让 C++ 可以读写它

/*verilator lint_off <msgs>*/
										关闭静态语法检测 
/*verilator lint_on <msgs>*/
```
