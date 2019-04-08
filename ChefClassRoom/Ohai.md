## How to collect the information of nodes

### Ohai
* is a tool to collect the information of node.\
* whenever convergance happens ohai is executed
* ohai returns the complete information in the form of ruby dictionary. (Json)
* To use info in cookbook use __node__ object
```
node['os_family']
```