FROM ubuntu:16.04

RUN apt-get update -y
RUN apt-get install -y vim wget git

RUN wget https://dl.google.com/go/go1.12.5.linux-amd64.tar.gz
RUN tar -C /usr/local -xzf go1.12.5.linux-amd64.tar.gz

WORKDIR /go/src/kaushikc92

ENV GOPATH /go
ENV PATH $GOPATH/bin:/usr/local/go/bin:$PATH

RUN go get github.com/derekparker/delve/cmd/dlv

CMD ["sh", "-c", "/bin/bash"]
