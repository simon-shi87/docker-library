FROM ubuntu:latest

RUN apt-get update -y && apt-get upgrade -y
RUN apt-get install -y tzdata curl ca-certificates && ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime && update-ca-certificates