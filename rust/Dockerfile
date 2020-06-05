FROM rust:1.43.1

RUN apt-get update

RUN apt-get install libssl-dev pkg-config -y

RUN curl -fsSL https://get.docker.com -o get-docker.sh

RUN sh get-docker.sh