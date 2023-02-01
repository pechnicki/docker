FROM jenkins/jenkins:latest

USER root
RUN apt update -y
# PYTHON
RUN apt install -y python3-pip
RUN pip3 install awscli --upgrade
# AWS CLI
RUN curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
RUN unzip awscliv2.zip
RUN ./aws/install
# NODE
RUN apt-get install -y nodejs