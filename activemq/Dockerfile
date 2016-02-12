FROM java:8-jdk
WORKDIR /opt/activemq
RUN wget -qO- http://ftp.unicamp.br/pub/apache/activemq/5.13.1/apache-activemq-5.13.1-bin.tar.gz | \
    tar xvz -C /opt/activemq --strip-components 1
EXPOSE 8161
EXPOSE 61616
ENTRYPOINT ["bin/activemq", "console"]
