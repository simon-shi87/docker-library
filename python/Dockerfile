FROM python:3.9.5-slim
EXPOSE 8000
ENV LANG en_US.UTF-8
ENV TZ=Asia/Shanghai
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
RUN sed -i "s@http://deb.debian.org@http://mirrors.aliyun.com@g" /etc/apt/sources.list &&  rm -Rf /var/lib/apt/lists/*
RUN apt-get update && apt-get install -y  iputils-ping git
COPY kubectl .
RUN chmod +x ./kubectl && mv ./kubectl /usr/local/bin/kubectl && chmod 777 *