FROM ubuntu:18.04

RUN apt-get update && \
    apt-get install -y software-properties-common git wget \
    iproute2 iputils-ping network-manager lsof ufw

RUN add-apt-repository ppa:bitcoin-abc/ppa && \
    add-apt-repository -y ppa:ubuntu-toolchain-r/test

RUN apt-get update && \
    apt-get install -y libstdc++-7-dev bitcoind
