FROM microbox/scratch

MAINTAINER e2tox <e2tox@microbox.io>

ADD rootfs.tar /
ADD influxdb.conf /etc/

WORKDIR /data

VOLUME /data

# Define default command.
EXPOSE 8083 8086
ENTRYPOINT ["/usr/bin/influxd"]
CMD ["-config", "/etc/influxdb.conf"]