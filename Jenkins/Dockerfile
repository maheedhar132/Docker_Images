FROM centos
RUN yum update -y && \
    yum upgrade -y
RUN wget -O /etc/yum.repos.d/jenkins.repo \
    https://pkg.jenkins.io/redhat-stable/jenkins.repo && \
    rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io.key && \
    yum upgrade && \
    yum install java-11-openjdk && \
    yum install jenkins && \
    systemctl daemon-reload
