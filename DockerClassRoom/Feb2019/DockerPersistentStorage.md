## Persistent Storage in Docker Containers

### Ideal Scenario

* Spin up a container
    * isolated area
    * required for apps to work
* States
    * Running
    * Stopped
    * Terminated(everything is lost)

        * Lets create a continer alpine
        * create a file
        * stop the container
        * start the container
        * is the file still available ?
        * terminate the container
    * Ephemeral & Immutable

    * What if i want some data(files/folders) from container even after terminating
        This is possible with docker  volume

    * Volume is about persistent storage
    * docker has aspecial command for this
        docker volume
          => create
          => delete
          => attach

    * Writing a Image storage which is crtical
    ```
    FROM tomcat:8
    ADD <source> <destination>
    VOLUME /usr/local/tomcat
    EXPOSE 8080
    CMD ["catalina.sh", "run"]
    ```

    * Running container
        => logs
             => container logs
             => application logs
                  stdout, stderr