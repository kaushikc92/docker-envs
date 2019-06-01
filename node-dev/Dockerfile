FROM ubuntu:latest

RUN apt-get update -y
RUN apt-get install -y vim git curl

RUN curl -sL https://deb.nodesource.com/setup_10.x | bash -
RUN apt-get install -y nodejs

WORKDIR /code

RUN git clone https://github.com/picolonet/parse-server
WORKDIR /code/parse-server
RUN npm install

CMD ["sh", "-c", "/bin/bash"]
