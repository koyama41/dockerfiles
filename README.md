# koyama41's dockerfiles

This is my experimental area.

For example,

    FROM ubuntu:14.04
    MAINTAINER KOYAMA Youichi <koyama41@gmail.com>
    WORKDIR /
    RUN apt-get update && apt-get -y upgrade
    RUN apt-get -y install unbound

(from ubuntu14.04-unbound/Dockerfile)

if you'd like to build the docker image above, try:

> **%** *git clone https://github.com/koyama41/dockerfiles.git*

> **%** *cd dockerfiles*

> **%** *cd ubuntu14.04-unbound*

> **%** *docker build .*
