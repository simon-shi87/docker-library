ARG NODE_VERSION=10.19.0

FROM mhart/alpine-node:$NODE_VERSION

MAINTAINER Simon "simon.shi@treelab.co"

RUN sed -i 's/dl-cdn.alpinelinux.org/mirrors.tuna.tsinghua.edu.cn/g' /etc/apk/repositories \
  && apk update --no-cache \
  && export PKGS="git docker openssh-client make gcc g++ python linux-headers paxctl libgcc libstdc++ bash curl tzdata" \
  && apk add --no-cache $PKGS \
  && apk add --no-cache libc6-compat \
  && echo "${TZ}" > /etc/timezone \
  && ln -sf /usr/share/zoneinfo/${TZ} /etc/localtime 

RUN npm i yarn typescript next -g
