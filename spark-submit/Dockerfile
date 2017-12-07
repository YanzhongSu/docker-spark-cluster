#Spark Submit Shell
FROM ubuntu

RUN apt-get update && apt-get install -y \
 wget \
 default-jdk \
 python3.6 \
 scala && cd /home && mkdir spark && cd spark && \
 wget http://ftp.unicamp.br/pub/apache/spark/spark-2.2.0/spark-2.2.0-bin-hadoop2.7.tgz && \
 tar -xvf spark-2.2.0-bin-hadoop2.7.tgz

ENV JAVA_HOME /usr/lib/jvm/java-1.8.0-openjdk-amd64
ENV SPARK_HOME /home/spark/spark-2.2.0-bin-hadoop2.7
ENV PYSPARK_PYTHON python3.6
ENV PATH $PATH:$SPARK_HOME/bin

