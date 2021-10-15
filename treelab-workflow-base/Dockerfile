FROM registry.cn-zhangjiakou.aliyuncs.com/caminer/golang:1.16.5

RUN apt-get update

RUN apt-get install autoconf automake libtool curl make g++ unzip -y
RUN git clone https://github.com/google/protobuf.git

RUN cd ./protobuf && bash ./autogen.sh && ./configure && make && make install && ldconfig

ENV GOPROXY=https://goproxy.cn
RUN go get -u github.com/golang/protobuf/protoc-gen-go