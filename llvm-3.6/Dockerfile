FROM ubuntu:16.04
WORKDIR /
RUN apt-get update
RUN \
 apt-get install -y ninja-build cmake clang python curl xz-utils --no-install-recommends && \
 curl http://llvm.org/releases/3.6.2/llvm-3.6.2.src.tar.xz | tar xJf - && \
 mv /llvm-3.6.2.src /llvm && \
 curl http://llvm.org/releases/3.6.2/compiler-rt-3.6.2.src.tar.xz | tar xJf - && \
 mv /compiler-rt-3.6.2.src /llvm/projects/compiler-rt && \
 curl http://llvm.org/releases/3.6.2/cfe-3.6.2.src.tar.xz | tar xJf - && \
 mv /cfe-3.6.2.src /llvm/tools/clang && \
 mkdir llvm/build && cd llvm/build && \
 CC=clang CXX=clang++ cmake -G Ninja .. && \
 ninja && \
 ninja install && \
 rm -rf /llvm /build && \
 strip /usr/local/bin/[a-fh-z]* && \
 apt-get remove --auto-remove -y ninja-build cmake clang curl xz-utils
