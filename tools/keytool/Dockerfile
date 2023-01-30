FROM alpine:3.17

RUN apk update && \
    apk add openjdk17-jre && \
    apk add openssl

RUN rm -rf /var/cache/apk/*
