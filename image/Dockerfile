FROM ubuntu:20.04

RUN mkdir /node
WORKDIR /node

RUN apt update && apt install wget curl -y
RUN wget https://github.com/ava-labs/avalanchego/releases/download/v1.7.7/avalanchego-linux-amd64-v1.7.7.tar.gz
RUN tar -xvf avalanchego-linux-amd64-v1.7.7.tar.gz

ENTRYPOINT [ "/node/avalanchego-v1.7.7/avalanchego" ]
