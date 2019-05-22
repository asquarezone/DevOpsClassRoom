# Terraform Modules

## What is a module?
* Reusable Terraform script is called as module.
* To create a module there is nothing special.
* Any terraform script can become a module
    * All of variables will become arguments
    * all of output section will become attributes

## Custom Modules
* Every module has source
* source should be local path of your terraform reusable directory(module) or terraform registry
* init shouldnot be done in modules
