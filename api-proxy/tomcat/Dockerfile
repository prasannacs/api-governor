# Set the base image to Ubuntu
FROM ubuntu

# File Author 
MAINTAINER prasannacs

# Update the repository source list
RUN apt-get update

######### JDK INSTALLATION ##########
RUN apt-get install oracle-java8

######### BEGIN TOMCAT INSTALLATION ##########
RUN echo groupadd tomcat
RUN echo useradd -s /bin/false -g tomcat -d /opt/tomcat tomcat



