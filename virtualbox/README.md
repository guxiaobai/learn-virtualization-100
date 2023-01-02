# Oracle VM VirtualBox

本期版本 | 上期版本
:---: | :---:
`Mon Jan  2 00:36:32 CST 2023` | -


## macOS

> `Monterey`

```bash
brew install virtualbox
```

## Ubuntu


```bash
domain=http://mirrors.tuna.tsinghua.edu.cn
name=/etc/apt/sources.list.d/virtualbox.list
keyrings=/usr/share/keyrings/oracle-virtualbox-2016.gpg

sudo apt-get update && sudo apt-get install -y lsb-release wget

wget -O- https://www.virtualbox.org/download/oracle_vbox_2016.asc | sudo gpg --dearmor --yes --output ${keyrings}
echo "deb [arch=amd64 signed-by=${keyrings}] ${domain}/virtualbox/apt/ $(lsb_release -cs) contrib" | sudo tee ${name}
sudo apt-get update && sudo apt-get install -y virtualbox-7.0
```

```bash
sudo rm -f ${name}
```


## VirtualBox Extension Pack

> `latest=$(VBoxManage -v | awk -Fr '{print $1}')`

```bash
latest=$(wget -q ${domain}/virtualbox/LATEST.TXT -O-)
extension=Oracle_VM_VirtualBox_Extension_Pack-${latest}.vbox-extpack

wget ${domain}/virtualbox/${latest}/${extension}
sudo VBoxManage extpack install --replace ${extension}
```

```bash
rm -f ${extension}
```


## Ref

* [https://www.virtualbox.org/](https://www.virtualbox.org/)
* [VirtualBox 镜像使用帮助 - 清华大学开源软件镜像站](https://mirrors.tuna.tsinghua.edu.cn/help/virtualbox/)