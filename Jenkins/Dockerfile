FROM amazonlinux:latest
RUN amazon-linux-extras install java-openjdk11 -y && \
    yum install wget -y && \
    mkdir /jenkins
WORKDIR /jenkins
RUN wget -O /etc/yum.repos.d/jenkins.repo http://pkg.jenkins-ci.org/redhat-stable/jenkins.repo && \
    rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io.key && \
    yum install jenkins -y && \
    systemctl start jenkins && \
    systemctl status jenikins
    
