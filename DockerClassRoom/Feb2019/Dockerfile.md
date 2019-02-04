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
 
