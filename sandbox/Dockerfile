FROM ubuntu

RUN apt-get update && \
apt-get install -y vim curl net-tools iputils-ping

WORKDIR /sandbox

VOLUME /sandbox

EXPOSE 22
EXPOSE 80
EXPOSE 8080
EXPOSE 8081
EXPOSE 3000

CMD tail -f /dev/null
