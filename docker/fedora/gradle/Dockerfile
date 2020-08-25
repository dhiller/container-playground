FROM amd64/fedora:31

RUN dnf install -y wget unzip java-1.8.0-openjdk
RUN wget https://services.gradle.org/distributions/gradle-6.6-bin.zip
RUN mkdir /opt/gradle
RUN unzip -d /opt/gradle gradle-6.6-bin.zip
RUN echo 'export JAVA_HOME=$(readlink -f /usr/bin/java | sed "s:/bin/java::")' >> $HOME/.bashrc
RUN echo 'export PATH=$PATH:/opt/gradle/gradle-6.6/bin' >> $HOME/.bashrc
