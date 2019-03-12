FROM ubuntu:latest as intermediate
MAINTAINER Tyler Akins <fidian@rumkin.com>

ENV LC_ALL C

COPY apple-bash/bin/* \
    bash/bin/* \
    dash/bin/* \
    fish/bin/* \
    zsh/bin/* \
    containers/multishell/update-links /usr/local/bin/

RUN bash /usr/local/bin/update-links
