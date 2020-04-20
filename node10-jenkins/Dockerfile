FROM node:10-slim

MAINTAINER Simon "simon.shi@treelab.co"

RUN apk update --no-cache \
  && export PKGS="git docker openssh-client make gcc g++ python linux-headers paxctl libgcc libstdc++ bash curl" \
  && apk add --no-cache $PKGS \
  && apk add --no-cache libc6-compat

RUN npm i yarn typescript next -g
