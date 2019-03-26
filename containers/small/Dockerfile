FROM ubuntu:latest as intermediate
COPY --from=fidian/multishell-apple-bash:latest \
    /usr/local/bin/apple-bash-97 \
    /usr/local/bin/apple-bash-106.220.2 \
    /usr/local/bin/
COPY --from=fidian/multishell-bash:latest \
    /usr/local/bin/bash-2.05.0 \
    /usr/local/bin/bash-3.1.23 \
    /usr/local/bin/bash-3.2.57 \
    /usr/local/bin/bash-4.0.44 \
    /usr/local/bin/bash-4.1.17 \
    /usr/local/bin/bash-4.2.53 \
    /usr/local/bin/bash-4.3.48 \
    /usr/local/bin/bash-4.4.23 \
    /usr/local/bin/bash-5.0.2 \
    /usr/local/bin/
COPY --from=fidian/multishell-dash:latest \
    /usr/local/bin/dash-0.5.10.2 \
    /usr/local/bin/
COPY --from=fidian/multishell-fish:latest  \
    /usr/local/bin/fish-1.23.1 \
    /usr/local/bin/fish-2.7.1 \
    /usr/local/bin/fish-3.0.2 \
    /usr/local/bin/
COPY --from=fidian/multishell-sash:latest  \
    /usr/local/bin/sash-3.8 \
    /usr/local/bin/
COPY --from=fidian/multishell-tcsh:latest \
    /usr/local/bin/tcsh-6.17.10 \
    /usr/local/bin/tcsh-6.18.05 \
    /usr/local/bin/tcsh-6.19.01 \
    /usr/local/bin/tcsh-6.20.00 \
    /usr/local/bin/
COPY --from=fidian/multishell-zsh:latest \
    /usr/local/bin/zsh-3.1.9 \
    /usr/local/bin/zsh-4.2.7 \
    /usr/local/bin/zsh-5.0.8 \
    /usr/local/bin/zsh-5.1.1 \
    /usr/local/bin/zsh-5.2 \
    /usr/local/bin/zsh-5.3.1 \
    /usr/local/bin/zsh-5.4.2 \
    /usr/local/bin/zsh-5.5.1 \
    /usr/local/bin/zsh-5.6.1 \
    /usr/local/bin/zsh-5.7.1 \
    /usr/local/bin/
COPY update-links /usr/local/bin
RUN /usr/local/bin/update-links && rm /usr/local/bin/update-links

FROM ubuntu:latest
MAINTAINER Tyler Akins <fidian@rumkin.com>
ENV LC_ALL C
COPY --from=intermediate /usr/local/bin/ /usr/local/bin/
