FROM rust:1.47.0

WORKDIR /usr/src/dgraph-ws-client

RUN apt-get update

RUN apt-get install libssl-dev pkg-config vim -y

RUN curl -fsSL https://get.docker.com -o get-docker.sh

RUN sh get-docker.sh
