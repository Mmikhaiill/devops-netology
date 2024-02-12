Задача 1.
    Опишите основные преимущества применения на практике IaaC-паттернов.

    Ценность IaC стоит на 3 китах: цена, скорость и уменьшение рисков. Уменьшение расходов относится не только к финансовой составляющей, но и к количеству времени, затрачиваемого на рутинные операции. Принципы IaC позволяют не фокусироваться на рутине, а заниматься более важными задачами. Автоматизация инфраструктуры позволяет эффективнее использовать существующие ресурсы. Также автоматизация позволяет минимизировать риск возникновения человеческой ошибки. Всё это является частью культуры DevOps, сочетающей в себе разработку и операции

Задача 2.
    Чем Ansible выгодно отличается от других систем управление конфигурациями?
        - Низкий порог вхождения
        - Отсутствие агента
        - Минимальные требования к хостам
        - Идемпотентность
        - YAML

    Какой, на ваш взгляд, метод работы систем конфигурации более надёжный — push или pull?
        - Я считаю, что более надежным является pull, т.к. все изменения применяются изнутри кластера. Подобный процесс весьма безопасен, поскольку ни у одного внешнего клиента нет доступа к правам администратора кластера.

Задача 3.

VirtualBox:

machine@imachine:~$ virtualbox --help
Oracle VM VirtualBox VM Selector v6.1.26_Ubuntu
(C) 2005-2021 Oracle Corporation
All rights reserved.

No special options.

If you are looking for --startvm and related options, you need to use VirtualBoxVM.

Vagrant
machine@imachine:~$ vagrant --version
Vagrant 2.2.18

Ansible
machine@imachine:~$ ansible --version
ansible 2.9.6
  config file = /etc/ansible/ansible.cfg
  configured module search path = ['/home/machine/.ansible/plugins/modules', '/usr/share/ansible/plugins/modules']
  ansible python module location = /usr/lib/python3/dist-packages/ansible
  executable location = /usr/bin/ansible
  python version = 3.8.10 (default, Sep 28 2021, 16:10:42) [GCC 9.3.0]


Задача 4.

machine@imachine:~/all_vagrant/vagrant$ vagrant ssh
Welcome to Ubuntu 20.04.2 LTS (GNU/Linux 5.4.0-80-generic x86_64)

* Documentation:  <https://help.ubuntu.com>
* Management:     <https://landscape.canonical.com>
* Support:        <https://ubuntu.com/advantage>

  System information as of Wed 03 Nov 2021 09:11:28 AM UTC

  System load:  0.0               Users logged in:          0
  Usage of /:   3.2% of 61.31GB   IPv4 address for docker0: 172.17.0.1
  Memory usage: 20%               IPv4 address for eth0:    10.0.2.15
  Swap usage:   0%                IPv4 address for eth1:    192.168.192.11
  Processes:    103

This system is built by the Bento project by Chef Software
More information can be found at <https://github.com/chef/bento>
Last login: Wed Nov  3 09:10:56 2021 from 10.0.2.2
vagrant@server1:~$ docker ps
CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES

