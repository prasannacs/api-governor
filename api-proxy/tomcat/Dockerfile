# Set the base image to Ubuntu
FROM ubuntu

# File Author 
MAINTAINER prasannacs

# Update the repository source list
RUN apt-get update

######### JDK INSTALLATION ##########
RUN apt-get update && \
    apt-get upgrade -y && \
    apt-get install -y  software-properties-common && \
    add-apt-repository ppa:webupd8team/java -y && \
    apt-get update && \
    echo oracle-java7-installer shared/accepted-oracle-license-v1-1 select true | /usr/bin/debconf-set-selections && \
    apt-get install -y oracle-java7-installer && \
    apt-get clean

######### BEGIN TOMCAT INSTALLATION ##########
RUN echo groupadd tomcat
RUN echo useradd -s /bin/false -g tomcat -d /opt/tomcat tomcat



