ansible-dev-computer
===================

This repository contains Ansible scripts to reinstall a PHP developer computer.

Requirements
------------

```
sudo apt-get install ansible
```
or (to get the last version of Ansible)

```
$ sudo apt-get update
$ sudo apt-get install software-properties-common
$ sudo apt-add-repository --yes --update ppa:ansible/ansible
$ sudo apt-get install ansible
```

```
$ git clone git@github.com:franek/ansible-dev-computer.git

```

Add into /etc/ansible/hosts

```
localhost ansible_connection=local
```

Usage
-----

```
ansible-galaxy install -r requirements.yml
ansible-playbook -l localhost playbook.yml --ask-sudo-pass
```
