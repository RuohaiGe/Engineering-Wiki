## Common command

```bash
gdb ./${program_name} core
```

- core 可以显示更多seg-fault的原因
- b xxx (设置断点)
- r 跑，到b停
- s (一步一步看）
- c 调到breakpoint
- n (一步一步，不进入函数)
- bt (可以看到哪里有问题)

## Python GDB

```bash
gdb python
(gdb) run /path/to/script.py
## wait for segfault ##
(gdb) backtrace
## stack trace of the c code
```
