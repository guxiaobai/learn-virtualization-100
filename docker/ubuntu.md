# Install Docker Engine on Ubuntu

|本期版本| 上期版本
|:---:|:---:
`Mon Jan  2 01:57:24 CST 2023` | -

> `22.04`

```bash
domain=https://mirrors.tuna.tsinghua.edu.cn/docker-ce/linux/ubuntu
keyrings=/usr/share/keyrings/docker-archive-keyring.gpg
name=/etc/apt/sources.list.d/docker.list

sudo apt-get update && sudo apt-get install -y lsb-release wget

wget -O- ${domain}/gpg | sudo gpg --dearmor --yes --output ${keyrings}
echo "deb [arch=amd64 signed-by=${keyrings}] ${domain} $(lsb_release -cs) stable" | sudo tee ${name}
sudo apt-get update && sudo apt-get install -y docker-ce
```

```bash
sudo rm -f ${name}
```

> 用户权限

```bash
sudo usermod -aG docker $USER
```

> 开机启动

```
sudo systemctl enable docker && sudo systemctl start docker
```

> 镜像加速

```
sudo tee -a /etc/docker/daemon.json > /dev/null <<EOF
{
  "registry-mirrors": [
    "https://hub-mirror.c.163.com",
    "https://mirror.baidubce.com"
  ]
}
EOF
```

```
sudo systemctl daemon-reload && sudo systemctl restart docker
```



## Install the Compose standalone

```
wget https://github.com/docker/compose/releases/download/v2.14.2/docker-compose-linux-x86_64 -O /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
```


## Ref

* [https://docs.docker.com/engine/install/ubuntu/](https://docs.docker.com/engine/install/ubuntu/)
* [https://yeasy.gitbook.io/docker_practice/install/ubuntu](https://yeasy.gitbook.io/docker_practice/install/ubuntu)
* [https://yeasy.gitbook.io/docker_practice/compose/install](https://yeasy.gitbook.io/docker_practice/compose/install)
* [Docker Community Edition 镜像使用帮助](https://mirrors.tuna.tsinghua.edu.cn/help/docker-ce/)