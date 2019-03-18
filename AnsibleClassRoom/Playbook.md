# Ansible Playbooks

* Play book is declarative syntax of getting things done with ansible
* Playbook is expressed in YAML
* Basic structure is as follows
```

---
- hosts: #where it has to execute
  become: # run this as sudo user
  tasks:
    - name: "name your task"
      <module_name>:
         <parameter name>: <value>

```

* Example

```

---
- hosts: all
  become: yes
  tasks:
    - name: create file
      file:
        path: /home/ansible/1.txt
        state: present
    - name: delete the file
      file:
      path: /home/ansible/1.txt
      state: absent

```