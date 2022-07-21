FROM alpine:latest

ENV TZ=Asia/Shanghai

RUN apk add tzdata \
  && echo "${TZ}" > /etc/timezone \
  && ln -sf /usr/share/zoneinfo/${TZ} /etc/localtime \