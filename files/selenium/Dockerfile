FROM fedora

RUN yum install -y java-1.7.0-openjdk wget
RUN yum update -y
RUN wget http://selenium-release.storage.googleapis.com/2.41/selenium-server-standalone-2.41.0.jar
CMD ["java", "-jar", "selenium-server-standalone-2.41.0.jar", "-role", "hub"]
