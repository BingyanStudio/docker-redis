FROM alpine:3.3

ENV REDIS_VERSION 3.0.5

RUN apk update && \
    apk add 'redis<3.0.6' && \
    mkdir -p /data/redis && \
    rm -rf /var/cache/apk/*

WORKDIR /data/redis
VOLUME /data/redis
EXPOSE 6379

CMD ["redis-server"]
