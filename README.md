# koyama41's dockerfiles

This is my experimental area.

For example,

    FROM ubuntu:14.04
    MAINTAINER KOYAMA Youichi <koyama41@gmail.com>
    WORKDIR /
    RUN apt-get update && apt-get -y upgrade
    RUN apt-get -y install unbound

(from ubuntu14.04-unbound/Dockerfile)
  