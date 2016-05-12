FROM scratch

MAINTAINER Andreas Eiermann <andreas@hypriot.com>

COPY . /
ENV PATH=/:/usr/local/bin:$PATH

ENV SERVER_ADDR=:80 \
    PLUGIN_FILTER=plugins/* \
    DATABASE_DRIVER=sqlite3 \
    DATABASE_CONFIG=/var/lib/drone/drone.sqlite \
    REMOTE_DRIVER=github

VOLUME /var/lib/drone
EXPOSE 80
ENTRYPOINT ["/usr/local/bin/drone"]
