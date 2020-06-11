FROM node:12.16.3-alpine

ENV TZ=Asia/Shanghai

RUN RUN sed -i 's/dl-cdn.alpinelinux.org/mirrors.tuna.tsinghua.edu.cn/g' /etc/apk/repositories \
  && apk update --no-cache \
  && apk add tzdata \
  && echo "${TZ}" > /etc/timezone \
  && ln -sf /usr/share/zoneinfo/${TZ} /etc/localtime \
  && rm /var/cache/apk/*