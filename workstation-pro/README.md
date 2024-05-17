# VMware Workstation Pro

|本期版本| 上期版本
|:---:|:---:
`Thu Mar 14 19:49:42 CST 2024` | -

## License

Key | Version
:---: | :---:
`JU090-6039P-08409-8J0QH-2YR7F` | [17.0.0](https://download3.vmware.com/software/WKST-1700-WIN/VMware-workstation-full-17.0.0-20800274.exe)
`ZF3R0-FHED2-M80TY-8QYGC-NPKYF` | [16.1.2](https://download3.vmware.com/software/wkst/file/VMware-workstation-full-16.1.2-17966106.exe)


## VMware Tools

```bash
sudo apt-get install -y open-vm-tools-desktop
```

* [如何安装 VMware Tools (1014294)](https://kb.vmware.com/s/article/1014294?lang=zh_CN)
* [在 Ubuntu 虚拟机中安装 VMware Tools (1022525)](https://kb.vmware.com/s/article/1022525?lang=zh_cn)
* [VMware 对 open-vm-tools 的支持 (2073803)](https://kb.vmware.com/s/article/2073803)


## macOS


## Ref

* <https://github.com/DrDonk/unlocker>
* <https://github.com/kholia/OSX-KVM>

```
# Convert DMG to CDR or ISO with Disk Utility | OSXDaily
hdiutil convert ./BigSur-full.dmg -format UDTO -o ./a.iso
```




* ~~<https://github.com/netgc/esxi-unlocker>~~
* <https://sysin.org/blog/how-to-install-macos/>

> `.vmx`

```
smc.version = "0"
hw.model.reflectHost = "FALSE"
hw.model = "Macmini8,1"
board-id.reflectHost = "FALSE"
board-id = "Mac-7BA5B2DFE22DDD8C"
serialNumber.reflectHost = "FALSE"
serialNumber = "C07W1059JYVX"
ethernet0.virtualDev = "vmxnet3"
```


## Ref

* [https://www.vmware.com/products/workstation-pro.html](https://www.vmware.com/products/workstation-pro.html)
* [https://www.isharepc.com/36181.html](https://www.isharepc.com/36181.html)
* [VMware Workstation Pro 文档](https://docs.vmware.com/cn/VMware-Workstation-Pro/index.html)
* [两款 VMware 虚拟机一键去虚拟化工具](https://xiaoyi.vc/vmware-se.html)
* [博通放大招：VM Workstation Pro免费了](https://mp.weixin.qq.com/s/B2QE4DSMPLTeGx4VtUiokw)