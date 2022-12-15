FROM ubuntu
RUN apt-get update -y && \
    apt-get upgrade -y && \
    apt-get install wget -y && \
    wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key |sudo gpg --dearmor -o /usr/share/keyrings/jenkins.gpg