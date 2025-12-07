## Variable
```yaml
SHELL:											set shell
```
## Syntax
```yaml
@:												suppress echoing
-:												ignore errors
+:							
$(),${}:						 				variable reference
$(function arguments) ${function arguments}:	Function Call
.PHONY:											该命令非文件名时使用，防止和文件名冲突
```
## Options
```yaml
-n --just-print:								only echoes most recipes, without executing them
-j --jobs:							 			Parallel Execution
-C DIRECTORY, --directory=DIRECTORY:			去到指定目录读取 makefile
```
## Debug
```verilator
make -C ./build/obj_dir/ -f Vtop.mk print
print:
	@ehco	"$(VK_USER_OBJS) $(VK_GLOBAL_OBJS) $(VM_PREFIX)__ALL.a"		打印verilator信息	
```
```text
print:
	@ehco	""
	@ehco	""
```
