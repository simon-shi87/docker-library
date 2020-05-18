FROM node:12-alpine

RUN sed -i 's/dl-cdn.alpinelinux.org/mirrors.tuna.tsinghua.edu.cn/g' /etc/apk/repositories \
  && apk update --no-cache \
  && apk add --no-cache libc6-compat \
  && apk add --no-cache bash

