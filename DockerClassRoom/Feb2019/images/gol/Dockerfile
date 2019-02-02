FROM tomcat:8
LABEL "AUTHOR"="qtkhaja@gmail.com"
ADD  https://s3-us-west-2.amazonaws.com/qt-binaries/gameoflife.war /usr/local/tomcat/webapps/gameoflife.war
EXPOSE 8080
CMD ["catalina.sh", "run"]