## Jenkins Node Setup

### How

#### SSH
1. Linux Master communicates to Linux Slave

##### HOW
1. On Slave, Create a user (prefer same username as what is used in jenkins master)
```
adduser jenkins
```
2. Give Sudo permissions if required
```
visudo
jenkins ..........................
```
3. Log in into jenkins master
4. create a ssh key for jenkins master
```
ssh-keygen
```
5. copy the public key of jenkins master to jenkins slave
```
ssh-copy-id jenkins@<jenkinsslaveip>
```
6. Test if it works
```
ssh <jenkinsslaveip>
```

### Agent (Linux Master => Windows Slave)
1. Windows Slave communicates to Linux Master
2. Enable something in Settings