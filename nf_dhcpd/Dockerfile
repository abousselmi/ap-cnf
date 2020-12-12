FROM alpine:latest

RUN apk add -U dhcp tcpdump \
    && rm -rf /var/cache/apk/* \
    && touch /var/lib/dhcp/dhcpd.leases

VOLUME [ "/etc/dhcp/dhcpd.conf" ]
EXPOSE 67/udp 67/tcp

CMD [ "/usr/sbin/dhcpd", "-4", "-f", "-d", "--no-pid", "-cf", "/etc/dhcp/dhcpd.conf" ]
