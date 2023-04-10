FROM openjdk:17-oracle
RUN microdnf install yum
RUN yum install wget -y && \
    mkdir /jenkins
RUN yum install epel-release -y && \
    yum install npm -y && \
    yum install maven -y
WORKDIR /jenkins
RUN wget https://get.jenkins.io/war/2.399/jenkins.war
EXPOSE 8080
CMD java -jar jenkins.war
    
