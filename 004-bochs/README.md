# 004 - Bochs

**macOS**

* `brew install bochs`

**Ubuntu**

* `apt-get install vagbios bochs bochs-x bximage`

**创建磁盘**

* 软盘: `bximage -mode=create -fd=1.44M -q a.img`
* 硬盘: `bximage -mode=create -hd=10M -q c.img`

## Ref

* [https://bochs.sourceforge.io/](https://bochs.sourceforge.io/)
* [http://nongnu.org/vgabios/](http://nongnu.org/vgabios/)
* [Bochs简易教程](http://www.edu2act.cn/article/bochsjian-yi-jiao-cheng/)


**x86汇编语言 - 从实模式到保护模式**

* 5.9.2 Bochs 下的程序调试入门

* `s`: 单步执行
* `b`: 断点
* `c`: 持续执行
* `r`: 显示通用寄存器的内容
* `sreg`: 显示段寄存器
