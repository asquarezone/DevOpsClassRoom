# Ansible Setup & Configuration

## PreReq's
* Ansible control server has to be linux
* In this case node is also linux
* The above linux machines should be reachable (by network)


## Setup

* Admin user for ansible
```
# become root user
sudo -i
adduser ansible
```
* Changing key based authentication to also support password based authenticaion
```
nano /etc/ssh/sshd_config
# change passwordAuthentication from no to yes & save the file
service sshd restart
```
* Make ansible user admin
```
visudo
# scroll to the line where you see %sudo or wheel
# and add the below line
ansible (ALL:ALL) NOPASSWD:ALL

```
* Install Python & Ansible
    * Follow instructions [from here](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html#latest-releases-via-apt-ubuntu)
    