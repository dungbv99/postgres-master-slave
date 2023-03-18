FROM postgres:9.6-alpine
ENV GOSU_VERSION 1.10
COPY ./setup-master.sh /docker-entrypoint-initdb.d/setup-master.sh
ADD ./gosu /usr/bin/
RUN chmod +x /usr/bin/gosu
RUN chmod 0666 /docker-entrypoint-initdb.d/setup-master.sh
#RUN apt-get update && apt-get install --assume-yes ssh
