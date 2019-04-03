# vagrant_ansible_os_hardening
centos7, vagrant up, vagrant provision

## Prerequisites
```bash
VirtualBox (And Expansion pack when using a vbox image that uses USB3)
Vagrant
```
Using dev-sec's hardening repo's
```bash
git clone https://github.com/dev-sec/ansible-os-hardening roles/ansible-os-hardening
git clone https://github.com/dev-sec/ansible-ssh-hardening roles/ansible-ssh-hardening
```
## Launch vagrant box
```bash
vagrant up
```

## Enter Linux box
```bash
vagrant ssh
sudo su
```

## Apply Ansible provisioning
```bash
vagrant provision
```


## General
Don’t forget to shutdown/destroy the VM’s when done:
```bash
vagrant halt
```
or
```bash
vagrant destroy -f
```
