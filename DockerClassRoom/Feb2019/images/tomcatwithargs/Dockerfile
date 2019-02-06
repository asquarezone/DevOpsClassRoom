From tomcat:8
ADD sourceurl="https://qt.in/gameoflife.war"
ARG location="/var/lib/tomcat/gameoflife.war"
ADD $sourceurl $location
EXPOSE 8080
CMD ["catalina.sh", "run"]

