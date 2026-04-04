FROM tomcat:10-jdk17-temarin-jammy
RUN rm /usr/local/tomcat/conf/server.xml
COPY fdx-ui/server.xml /usr/local/tomcat/conf/server.xml
RUN rm -rf /usr/local/tomcat/webapps/ROOT/*
COPY fdx-backend/target/fdxbackendapi.war /usr/local/tomcat/webapps
ENTRYPOINT /usr/local/tomcat/bin/catalina.sh 

ENTYPOINT ["/usr/local/tomcat/bin/catalina.sh","run"]


