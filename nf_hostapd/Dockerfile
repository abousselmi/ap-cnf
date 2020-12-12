FROM ubuntu:18.04

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update \
    && apt-get install -y hostapd screen iproute2 nftables iptables \
        tcpdump iputils-ping \
    && rm -rf /var/lib/apt/lists/*

CMD [ "/bin/sleep", "infinity" ]
