FROM alpine:3.1

ENV REDIS_VERSION 2.8.23

RUN apk update && \
    apk add 'redis<2.8.24' && \
    mkdir -p /data/redis && \
    rm -rf /var/cache/apk/*

WORKDIR /data/redis
VOLUME /data/redis
EXPOSE 6379

CMD ["redis-server"]
