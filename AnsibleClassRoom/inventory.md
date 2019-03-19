# Ansible Inventory

* Inventory is list of nodes which ACS has to do CM
* Generally we might not want to execute some playbooks on all nodes
* Inventory uses ini file format
* default inventory is @ /etc/ansible/hosts
* custom inventory by using a argument "-i"
```
 ansible -m ping all
 # inventory will be picked up from /etc/ansible/hosts

 ansible -i myinventory -m ping all
```
* Inventories are of two types
    * Static Inventory
    * Dynamic Inventory

## Static Inventory
* statically writing down all the node dns(fqdn) or ipaddress
* There will be groups
```
[groupname]
<nodeip/dns>
<nodeip/dns>
```

## Activity

Configure Ansible control server to communicate with the 3 nodes
as shown below
![Preview](./images/ansibleactivity.png)

* Workbook items [Refer](https://github.com/asquarezone/ChefZone/blob/master/Workbook/nodejs/Workbooks.md)

  