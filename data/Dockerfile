FROM scratch

MAINTAINER Andreas Eiermann <andreas@hypriot.com>

COPY drone_static /usr/local/bin/drone
COPY etc /

ENV SERVER_ADDR=:80
ENV PLUGIN_FILTER=plugins/*
ENV DATABASE_DRIVER=sqlite3
ENV DATABASE_CONFIG=/var/lib/drone/drone.sqlite

ENV REMOTE_DRIVER=github

VOLUME /var/lib/drone
EXPOSE 80
ENTRYPOINT ["/usr/local/bin/drone"]
