FROM dockerfile/java
MAINTAINER Fawad Halim <fawad@fawad.net>

WORKDIR /tmp
RUN wget -O hazelcast.zip "http://download.hazelcast.com/download.jsp?version=hazelcast-3.2.4"
RUN unzip hazelcast.zip
RUN rm hazelcast.zip
RUN mv hazelcast* /opt/hazelcast

ENV HAZELCAST_HOME /opt/hazelcast

WORKDIR /opt/hazelcast/bin
CMD sh server.sh

EXPOSE 5701
