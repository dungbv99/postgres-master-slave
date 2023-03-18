FROM postgres:9.6-alpine
ENV GOSU_VERSION 1.10
ADD ./gosu /usr/bin/
RUN chmod +x /usr/bin/gosu
COPY ./setup-slave.sh /setup-slave.sh
RUN chmod +x /setup-slave.sh
ENTRYPOINT ["/setup-slave.sh"]
CMD ["gosu","postgres","postgres"]
