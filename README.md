### Demo setup Wordpress on Ubuntu 18/20 with Ansible

In Vagrantfile define Ubuntu version:
`config.vm.box = "ubuntu/bionic64"` for Ubuntu 18
`config.vm.box = "ubuntu/focal64"` for Ubuntu 20

Deploy Vagrant VM
```
vagrant up
```

define Vagrant external IP in /etc/hosts on host machine

define variables in vars/vagrant.yml


Deploy Wordpress
```
ansible-playbook -i hosts main.yml -e@vars/vagrant.yml
```