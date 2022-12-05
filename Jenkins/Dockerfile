FROM ubuntu
#RUN apt-get install jenkins
RUN apt update -y && \
    apt upgrade -y
RUN apt-get install wget
RUN wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | gpg --dearmor -o /usr/share/keyrings/jenkins.gpg
RUN sh -c 'echo deb [signed-by=/usr/share/keyrings/jenkins.gpg] http://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'
RUN apt update -y && \
    apt upgrade -y
