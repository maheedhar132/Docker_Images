FROM openjdk:21-oraclelinux8
RUN microdnf install yum
RUN yum install wget -y && \
    mkdir /jenkins
WORKDIR /jenkins
RUN wget -O /etc/yum.repos.d/jenkins.repo \
    https://pkg.jenkins.io/redhat-stable/jenkins.repo && \
    rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io-2023.key && \
    dnf upgrade -y && \
    dnf install jenkins -y
    
