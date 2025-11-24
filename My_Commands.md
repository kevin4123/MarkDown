## Git
```bash
git help <command>				# 帮助
git <command> -h				

git init
git config --local --list		# 当前仓库配置
git config --global --list		# 全局配置（当前用户的所有仓库）
git config --system --list		# 系统配置（系统所有用户）
git status						# Show the working tree status
git log							# Show commit logs
git add . && git commit -m "message" && git push
```
## Encode
```bash
chcp							# 查看当前编码
chcp 65001						# 修改为UTF-8
chcp 936						# 修改为GBK
```
## GDB
```bash
(gdb) target remote localhost:1234
(gdb) break _start                   # 在入口处设置断点
(gdb) continue                       # 运行到断点
(gdb) stepi                          # 单步执行一条指令
(gdb) info registers                 # 查看所有寄存器
(gdb) watch $x3                      # 监视 x3 的变化
```
## WSL
```bash
wsl								# 启动默认版本


```
## QEMU
```bash
qemu-system-riscv32 -machine virt -bios none -nographic -serial mon:stdio	# 开发板，串口->终端
# 调试控制台 
(qemu) Ctrl-A	+ C					# 启动控制台
(qemu) info registers				# 查看寄存器
(qemu) q							# 退出
(qemu) info mtree					# 查看内存映射信息
```
## RISCV
```bash
riscv32-unknown-elf-gcc -nostartfiles -nostdlib start.s -o start.elf		# 
```
