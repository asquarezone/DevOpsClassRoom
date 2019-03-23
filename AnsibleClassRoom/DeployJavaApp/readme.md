# Deploy java web app to tomcat

## Steps
1. Install suitable version of java (openjdk 8/openjdk 9)
2. Install suitable version of appserver(tomcat-8)
3. find the directory to copy the java web app (.war)
4. restart tomcat(appserver)

## Do this deployment of game of life 
[Download Link](https://github.com/QT-DevOps/DevOpsIssues/issues/45#issuecomment-399738259)


```
- hosts: appserver
  become: yes
  roles:
  - sometomcat
  tasks:
  - get_url:
      src: <locationof war file as http url>
      dest: <tomcat webapps direcory>
    notify:
    - restart tomcat
  handlers:
  - name: restart tomcat
```