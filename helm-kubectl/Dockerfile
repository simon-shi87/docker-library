FROM dtzar/helm-kubectl:3.9.3

RUN sed -i 's/dl-cdn.alpinelinux.org/mirrors.tuna.tsinghua.edu.cn/g' /etc/apk/repositories \
  && apk add aws-cli \
  && curl -LO https://storage.googleapis.com/kubernetes-release/release/v1.23.6/bin/darwin/amd64/kubectl \
  && chmod +x ./kubectl \
  && mv ./kubectl /usr/local/bin/kubectl
