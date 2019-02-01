## Introduce Images, Registry & Containers
* We need to create Docker Images
* To Create Docker Images 
    * Create a container & Take snapshot of it (not recommended)
    * Dockerfile Which we need to create
## How is it Working ?
* Container : Isolated Area

* History:
    dotCloud: PAAS Services 
        Test dc => docker
    Docker Inc

* NameSpaces: Isolations are created using Namespaces. 
* cgroups: Resource limits are imposed by cgroups

* Components:
   * client => docker cmd line
   * daemon
   * containerd
   * runc
   * compute services

* Windows Containers:
  * native containers
  * Hyperv isolations: (Security Benifits  & linux containers to run on windows)

* Windows:
   => Windows Server Core
   => Window Server Nano 

# Writing Docker files
  * need to know how to install/configure the application manually

  * Ubuntu server: I want to install apache2
   > sudo apt-get update && sudo apt-get install apache2 -y


   * FROM ubuntu:18
    RUN apt-get update && apt-get install apache2 -y
    CMD