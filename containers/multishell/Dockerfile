FROM ubuntu:latest as intermediate
MAINTAINER Tyler Akins <fidian@rumkin.com>

ENV LC_ALL C

COPY apple-bash/bin/* \
    bash/bin/* \
    dash/bin/* \
    fish/bin/* \
    zsh/bin/* \
    scripts/update-links /usr/local/bin/

RUN /usr/local/bin/update-links
