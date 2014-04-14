FROM bradrydzewski/base

WORKDIR /home/ubuntu
USER ubuntu
ENV JAVA_HOME /usr/lib/jvm/java-7-openjdk-amd64

RUN sudo apt-get -y install openjdk-7-jdk default-jdk        && \
    sudo apt-get -y install ant ant-contrib ivy gradle && \
    sudo update-java-alternatives -s java-1.7.0-openjdk-amd64 2> /dev/null


RUN cd /tmp && wget  http://apache.org/dist/maven/maven-3/3.2.1/binaries/apache-maven-3.2.1-bin.tar.gz
RUN cd /opt && sudo tar xzf /tmp/apache-maven-3.2.1-bin.tar.gz && sudo ln -fs /opt/apache-maven-3.2.1/bin/mvn /usr/bin/mvn
