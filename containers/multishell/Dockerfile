FROM fidian/multishell-scripts:latest
MAINTAINER Tyler Akins <fidian@rumkin.com>

ENV LC_ALL C
COPY --from=fidian/multishell-apple-bash:latest /usr/local/bin/ /usr/local/bin
COPY --from=fidian/multishell-apple-ksh93:latest /usr/local/bin/ /usr/local/bin
COPY --from=fidian/multishell-bash:latest /usr/local/bin/ /usr/local/bin
COPY --from=fidian/multishell-busybox:latest /usr/local/bin/ /usr/local/bin
COPY --from=fidian/multishell-dash:latest /usr/local/bin/ /usr/local/bin
COPY --from=fidian/multishell-fish:latest /usr/local/bin/ /usr/local/bin
COPY --from=fidian/multishell-ksh93:latest /usr/local/bin/ /usr/local/bin
COPY --from=fidian/multishell-sash:latest /usr/local/bin/ /usr/local/bin
COPY --from=fidian/multishell-tcsh:latest /usr/local/bin/ /usr/local/bin
COPY --from=fidian/multishell-zsh:latest /usr/local/bin/ /usr/local/bin
