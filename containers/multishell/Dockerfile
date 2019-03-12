FROM ubuntu:latest as intermediate

ENV LC_ALL C

COPY apple-bash/bin/* /usr/local/bin/
COPY bash/bin/* /usr/local/bin/
COPY fish/bin/* /usr/local/bin/

COPY containers/multishell/update-links /
RUN bash /update-links


FROM ubuntu:latest
MAINTAINER Tyler Akins <fidian@rumkin.com>
COPY --from=intermediate /usr/local/bin/ /usr/local/bin/
