FROM ubuntu:latest
RUN apt update && apt install -y \
    autoconf \
    bison \
    bsdmainutils \
    build-essential \
    cmake \
    doxygen \
    gdb \
    gettext \
    git \
    groff-base \
    libext2fs-dev \
    libncurses5-dev \
    libpcre2-dev \
    libxext-dev \
    libxt-dev \
    libz-dev \
    linux-headers-generic \
    ncurses-dev \
    perl \
    vim \
    xutils-dev

# Works with Alpine too
# FROM alpine:latest
# RUN apk add --no-cache build-base bash git bison

ENV LC_ALL C
CMD bash
