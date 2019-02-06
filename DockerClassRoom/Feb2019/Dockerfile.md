## Writing Dockerfile

* FROM => base image
* LABEL => Add metadocker
* RUN => instruction that will be executing while image is building
* ADD/COPY => 

* EXPOSE => 
    * WebServer => 80
    * AppServer => tomcat =>808
        * nodejs => developer any port
    * example: docker run -p 8080:8080 -p 50000:50000 jenkins

* CMD => can be overriten
* ENTRYPOINT => Freezes the application which gets started while you are running contaier
   exec format => ["echo", "hi], ["ls", "/var/lib"]

   Lifetime of your container => time which your cmd/entrypoint is alive
    CMD/ENTRYPOINT => should have someting which runs till your app is alive

   shell format => echo hi  / ls /var/libe
* ENV

## For tommorows disc
* ARG
* any other important
*
* Running containers in background mode (attached/detached)

Where to install application
/var/lib/tomcat/webapps

function add()
{
    return 3+5
}
 
function add(a,b)
{
    return a+b
}

Arguments can be called while building images
ENV => even after building images

USER Instruction => it creates the user & you will switch as user
> USER tomcat

WORKDIR INSTRCUTION => change your starting directory to some thing else

```
FROM ubuntu:trusty
RUN apt-get update && apt-get install git -y
USER git
WORKDIR /home/git
CMD ["echo", "hi"]
```

## Best Practices for Writing Docker files
* Dockerfile is a step by step process by manually doing 
  ```
  FROM alpine:3.9
  LABEL MAINTAINER="QT"
  RUN apk update && apk add openjdk8
  ENV JAVA_HOME="/usr/lib/jvm/"
  ARG downloadlocation
  ARG containerlocation
  ADD $downloadlocation $containerlocation
  EXPOSE 8088
  CMD ["java","-jar",$containerlocation]
  ```

* Your Dockerfile should be commited/placed at developers code (root directory of your code)

Steps for CI
*  Build COde
* Build Docker image
* Push docker image to registry