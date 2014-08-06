# Set the base image to Ubuntu
# kussj/java8
FROM ubuntu:14.04

# File Author / Maintainer
MAINTAINER kussj

# Update the repository sources list
RUN apt-get update

################## BEGIN INSTALLATION ######################

### Install Oracle Java ###
RUN apt-get install -y software-properties-common curl wget
RUN apt-add-repository -y ppa:webupd8team/java
RUN apt-get update
RUN echo oracle-java8-installer shared/accepted-oracle-license-v1-1 select true | sudo /usr/bin/debconf-set-selections
RUN apt-get install -y oracle-java8-installer