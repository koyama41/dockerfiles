FROM ubuntu:16.04
MAINTAINER KOYAMA Youichi <koyama@trans-nt.com>
WORKDIR /
RUN apt-get -y update && apt-get -y upgrade
RUN apt-get -y install zsh
RUN apt-get -y install binutils gcc make
RUN apt-get -y install cmake ninja-build
RUN apt-get -y install clang-3.9 clang-3.9-doc libclang-3.9-dev
RUN apt-get -y install git
RUN apt-get -y install libxml2-dev libxml2-utils xsltproc pkg-config
RUN apt-get -y install doxygen docbook
ENTRYPOINT [ "/usr/bin/zsh" ]
