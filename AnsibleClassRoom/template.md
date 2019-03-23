# Ansible Templates

## Usecases
* Creation of a file with some dynamic content
* Configuration Files: Template is answer for creating configuration

## How to create templates
* Understand Jinja2 templating

### Jinja2 
* Basic Syntax:
```
{{ expr }}
```

* Some examples
```
---
- hosts: all
  vars:
    my_msg: Welcome
  tasks:
  - name: print message
    debug:
      msg: "The message is : {{ my_msg }}. Os family is {{ ansible_os_family }}"
    
  - name: os family
    debug:
      var: ansible_os_family
```

## Behavior Parameters
[Refer](https://docs.ansible.com/ansible/latest/user_guide/intro_inventory.html#list-of-behavioral-inventory-parameters)


## Ansible Configurations
