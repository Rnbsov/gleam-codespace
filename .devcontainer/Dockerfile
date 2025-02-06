# syntax=docker/dockerfile:1.3-labs

FROM ghcr.io/void-linux/void-linux:20230204rc01-thin-x86_64

RUN xbps-install -u xbps && \
    xbps-install -Syu && \
    xbps-install -Sy bash less ncurses-base shadow curl python3 tar gzip findutils util-linux gleam erlang nodejs git && \
    chsh -s /bin/bash root || echo "chsh command failed, skipping" && \
    rm -rf /var/cache/xbps/

ENV HOME=/root

CMD [ "sleep", "infinity" ]
