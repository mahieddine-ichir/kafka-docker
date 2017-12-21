
FROM ubuntu:trusty
MAINTAINER mahieddine.ichir@gmail.com

ENV KAFKA_HOME /opt/kafka_2.11-1.0.0

ADD http://www-eu.apache.org/dist/kafka/1.0.0/kafka_2.11-1.0.0.tgz /opt/
RUN tar xfz /opt/kafka_2.11-1.0.0.tgz -C /opt/

RUN apt-get update -y && apt-get install -y default-jdk

ENTRYPOINT ["sh", "-c", "${KAFKA_HOME}/bin/zookeeper-server-start.sh ${KAFKA_HOME}/config/zookeeper.properties"]


