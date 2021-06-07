FROM jenkins/jenkins:lts
LABEL maintainer="rustam.mingazov@gmail.com"
USER root
RUN apt-get update && apt-get install -y docker.io && rm -rf /var/lib/apt/lists/*
RUN usermod -a -G docker jenkins
USER jenkins
EXPOSE 8080 
EXPOSE 50000