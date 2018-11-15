## EC2 pre-configuration

Set the follow command in the advance configuration for the EC2 instance.

```
#!/bin/bash
sudo yum update -y
sudo yum install git -y
sudo easy_install pip
sudo pip install ansible
```

## Ansible playook to instsall ADOP-C dependencies.

This playbook automates the process of packages installation and some configuration defined here

https://alm.accenture.com/wiki/display/DN/Standing+up+ADOP

The playbook was tested on this instance: CentOS Linux 7 x86_64 HVM EBS ENA 1804_1 - ami-08b08d6d

## Steps 

1. git clone https://robert.isla@innersource.accenture.com/scm/nadc/ansible-adopc-install-packages.git
2. cd adop-ansible
3. ansible-playbook main.yaml ( -vvv is optional to get more details)