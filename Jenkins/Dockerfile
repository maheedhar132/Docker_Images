FROM ubuntu
#RUN apt-get install jenkins
RUN apt update -y && \
    apt upgrade -y
RUN apt-get install wget -y
RUN apt-get install gnupg -y
RUN apt-get install gpg -y
RUN wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | gpg --dearmor -o /usr/share/keyrings/jenkins.gpg
RUN sh -c 'echo deb [signed-by=/usr/share/keyrings/jenkins.gpg] http://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'
RUN apt update -y && \
    apt upgrade -y
RUN apt-get install openjdk-11-jdk -y
RUN apt-get install jenkins -y
RUN service jenkins start
#keep docker container from exiting
ENTRYPOINT ["cat", "/var/log/jenkins/jenkins.log"]