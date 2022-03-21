### Demo setup Wordpress on Ubuntu 18 with Ansible


Deploy Vagrant VM with Ubuntu 18
```
vagrant up
```

define Vagrant external IP in hosts

define variables in vars/vagrant.yml


Deploy Wordpress
```
ansible-playbook -i hosts main.yml -e@vars/vagrant.yml
```