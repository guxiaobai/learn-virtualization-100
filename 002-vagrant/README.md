# 002 - Vagrant


## Boxes

* 获取下载地址: `curl https://app.vagrantup.com/ubuntu/boxes/focal64`


## Vagrantfile

* [`config.ssh.insert_key`](https://www.vagrantup.com/docs/vagrantfile/ssh_settings#config-ssh-insert_key)
* [Linked Clones](https://www.vagrantup.com/docs/providers/virtualbox/configuration#linked-clones)


## Wait cloud-init 

```
config.vm.provision "shell", inline: "sleep 60"
```


```
- name: Wait for clund-init
       wait_for:
         path: /var/log/cloud-init.log
         search_regex: running modules for final
```


## Ref

* [https://www.vagrantup.com/](https://www.vagrantup.com/)
* [https://cloud.centos.org](https://cloud.centos.org)
* [http://cloud-images.ubuntu.com/](http://cloud-images.ubuntu.com/) / [清华大学开源软件镜像站](https://mirrors.tuna.tsinghua.edu.cn/ubuntu-cloud-images/)
* [https://github.com/hashicorp/vagrant/issues/5571](https://github.com/hashicorp/vagrant/issues/5571)
