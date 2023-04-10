FROM adoptopenjdk/openjdk11
RUN microdnf install yum
RUN yum install wget -y && \
    mkdir /jenkins
WORKDIR /jenkins
RUN wget https://get.jenkins.io/war/2.399/jenkins.war
EXPOSE 8080
CMD java -jar jenkins.war
    
