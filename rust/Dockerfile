FROM rust:1.47.0
RUN rustup component add rustfmt --toolchain 1.47.0-x86_64-unknown-linux-gnu
WORKDIR /usr/src/dgraph-ws-client

RUN apt-get update

RUN apt-get install libssl-dev pkg-config vim -y

RUN curl -fsSL https://get.docker.com -o get-docker.sh

RUN sh get-docker.sh
