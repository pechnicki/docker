FROM jenkins/jenkins:latest

USER root
RUN apt-get update -y
# AWS CLI
RUN curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
RUN unzip awscliv2.zip
RUN ./aws/install
# NPM
RUN apt-get install -y npm
# NODE
RUN apt-get install -y nodejs
# ZIP
RUN apt-get install -y zip
# WGET
RUN apt-get install -y wget
# TERRAFORM
COPY install-terraform.sh .
RUN ./install-terraform.sh