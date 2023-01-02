# VHD

> 4.2.3 虚拟硬盘简介 - 《x86汇编语言 - 从实模式到保护模式》

```
# 4MB = 4 * 1024 * 1024 = 4194816D = 0400200H
# 4194816 - 512 = 4194304

VBoxManage createmedium disk --filename demo --format VHD --variant Fixed --size 4
hexdump -s 4194304 -n 512 -C demo.vhd
```