# Usage:
#
#     docker import - meshbox-base < bin/x86/openwrt-x86-generic-Generic-rootfs.tar.gz
#     docker build -t meshbox feeds/meshbox/docker/
#     container=$(docker run -d meshbox)
#     docker exec -i -t $container /bin/sh -c "uci get cjdns.cjdns.ipv6"
#     docker kill $container
#

FROM meshbox-base
MAINTAINER Lars Gierth <larsg@systemli.org>

ADD network /etc/config/network
ADD system /etc/config/system

# These end up setting kernel things we can't really set in docker
RUN ["busybox", "rm", "/etc/rc.d/S19firewall"]
RUN ["busybox", "rm", "/etc/rc.d/S60dnsmasq"]
RUN ["busybox", "rm", "/etc/rc.d/S11sysctl"]
RUN ["busybox", "rm", "/etc/rc.d/S98sysntpd"]

CMD ["/sbin/init"]
