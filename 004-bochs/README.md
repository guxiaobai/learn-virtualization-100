# 004 - Bochs

**macOS**

* `brew install bochs`

**Ubuntu**

* `apt-get install vagbios bochs bochs-x bximage`

**创建软盘**

* `bximage -mode=create -fd=1.44M -q a.img`

**创建硬盘**

* `bximage -mode=create -hd=10M -q c.img`

## Ref

* [https://bochs.sourceforge.io/](https://bochs.sourceforge.io/)
* [http://nongnu.org/vgabios/](http://nongnu.org/vgabios/)
* [Bochs简易教程](http://www.edu2act.cn/article/bochsjian-yi-jiao-cheng/)
