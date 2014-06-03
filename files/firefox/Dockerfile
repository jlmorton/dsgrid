FROM fedora

RUN yum install -y xorg-x11-server-Xvfb java-1.7.0-openjdk wget bzip2 dbus-glib firefox
RUN yum remove -y firefox
RUN yum update -y
RUN wget http://selenium-release.storage.googleapis.com/2.41/selenium-server-standalone-2.41.0.jar
RUN wget ftp://ftp.mozilla.org/pub/firefox/releases/25.0/linux-x86_64/en-US/firefox-25.0.tar.bz2
RUN tar -xjvf firefox-25.0.tar.bz2
ADD register-node.sh /var/register-node.sh
RUN chmod 755 /var/register-node.sh
CMD ["/bin/bash", "/var/register-node.sh"]
