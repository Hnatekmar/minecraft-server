FROM ubuntu:18.04

RUN apt-get update && \
    apt-get install -y wget openjdk-8-jdk unzip && \
    apt-get clean

WORKDIR /server

ADD server.zip .
RUN unzip server.zip && rm server.zip
RUN echo eula=true > eula.txt

CMD bash ServerStart.sh