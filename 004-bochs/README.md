# 004 - Bochs

**macOS**

* `brew install bochs`

**Ubuntu**

* `apt-get install vagbios bochs bochs-x bximage`

**创建磁盘**

* 软盘: `bximage -mode=create -fd=1.44M -q a.img`
* 硬盘: `bximage -mode=create -hd=10M -q c.img`

## Debug

* `s`: 单步执行
* `b`: 断点
* `c`: 持续执行
* `r`: 显示通用寄存器的内容
* `sreg`: 显示段寄存器
* `q`: 退出

<img src="xp.png" />

**Ref**

* 5.9.2 Bochs 下的程序调试入门 -  《x86汇编语言 - 从实模式到保护模式》
* [「Coding Master」第12话 如何正确的调试汇编程序](https://www.youtube.com/watch?v=EJgdGTAixVg&list=PLLBMaJy_MOpM2xUPbjSBSib7hUUaaEGa6&index=14)



## Ref

* [https://bochs.sourceforge.io/](https://bochs.sourceforge.io/)
* [http://nongnu.org/vgabios/](http://nongnu.org/vgabios/)
* [Bochs简易教程](http://www.edu2act.cn/article/bochsjian-yi-jiao-cheng/)


