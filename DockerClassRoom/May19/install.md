# Docker Installation

## Windows

* Windows 10 Non Home Editions and Windows Server 2016 and above:
    * Create native windows containers
    * Windows Containers as well as Linux Containers
    * [Refer](https://docs.docker.com/docker-for-windows/install/)
* Other Windows:
    * Virtual Box
    * Docker ToolBox
    * Dont install

## Linux
* simple Installation:
```
curl -fsSL https://get.docker.com -o get-docker.sh
 sh get-docker.sh
```

* Elaborate example

    * Create a linux machine in any cloud. In this example i would be using ubuntu 18
    * Login into linux & execute
    ```
    curl -fsSL https://get.docker.com -o get-docker.sh
    sh get-docker.sh
    ```
    * Install docker leads to creation of a group (linux group) __docker__
    * Members of __docker__ group will be able to speak to docker engine
    * __docker client__ will be accesible to all 
    * add your user to docker group and the logout
    ```
    sudo usermod -aG docker <username>
    ```