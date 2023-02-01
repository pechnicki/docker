FROM jenkins/jenkins:latest

USER root
RUN apt update -y
# AWS CLI
RUN curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
RUN unzip awscliv2.zip
RUN ./aws/install
# NODE
RUN apt install -y nodejs
# NPM
RUN apt install -y npm
# ZIP
RUN apt install -y zip
# TERRAFORM
CMD ["./install-terraform.sh"]