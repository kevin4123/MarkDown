## QEMU
```bash
qemu-system-riscv32 -machine virt -bios none -nographic -serial mon:stdio	# 开发板，串口->终端
# 调试控制台 
(qemu) Ctrl-A	+ C					# 启动控制台
(qemu) info registers				# 查看寄存器
(qemu) q							# 退出
(qemu) info mtree					# 查看内存映射信息
```