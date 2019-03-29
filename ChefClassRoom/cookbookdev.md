## Cookbook Development

### Steps
* Use chef generators to create cookbook.
* ensure you have chef extension installed in vscode

### Understanding
* Atomic unit of work in chef is resource
* syntax of resource
```
resourcetype 'name' do
   attribute 'value'
   action :type_of_action
end
```
* example 
```
# apt-get install git

package 'installing git' do
  package_name 'git'
  action :install
end
```

* Once you finish your cookbook dev, you should upload cookbook to chef server. This will be done by a chefdk component called as __berks__
    ```
    cd <cookbook>
    berks install
    berks upload
    ```

