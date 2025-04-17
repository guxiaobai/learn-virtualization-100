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

## vmware

组策略路径|	组策略设置|	值
---|---|---
计算机配置\管理模板\System\Device Guard|	启用基于虚拟化的安全性|	禁用

<img src="https://i-blog.csdnimg.cn/blog_migrate/49b71629642184a34510623ee4193a51.png" />

**Ref**

* [禁用 Hyper-V 以运行虚拟化软件 - Windows Client | Microsoft Learn](https://learn.microsoft.com/zh-cn/troubleshoot/windows-client/application-management/virtualization-apps-not-work-with-hyper-v#disable-device-guard-and-credential-guard)
* [配置 Credential Guard | Microsoft Learn](https://learn.microsoft.com/zh-cn/windows/security/identity-protection/credential-guard/configure?tabs=gpo#disable-credential-guard)
* [VMware与windows hyper-v的兼容性设置](https://blog.csdn.net/weixin_44537885/article/details/130985414)
* [windows10 禁用Device/Credential Guard解决方案](https://blog.csdn.net/qq_43355372/article/details/104923403)
* [为你的电脑关闭 Device/Credential Guard](https://answers.microsoft.com/zh-hans/windows/forum/all/%E4%B8%BA%E4%BD%A0%E7%9A%84%E7%94%B5%E8%84%91/a49978cb-cb26-44c9-ac49-54249dfba681)

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