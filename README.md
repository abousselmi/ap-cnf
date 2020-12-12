# AP CNF

Access Point (AP) cloud native function based on hostapd and dhcpd for the Edge.

## Prerequisites

- docker
- docker-compose

## Usage

Update `ap.env` file with you wireless device name.

> Note: make sure that you wireless card supports AP functions.

To start the AP, you simply do:

```console
$ sudo ./apctl start
```

## Implementation

- [x] Create two different containers for hostapd and dhcp
- [x] Use default docker networking
- [x] Use of screen to be able to access hostapd log
- [ ] Make dhcpd configuration dynamic


## Reference

This project gave me a lot of insight:

- https://github.com/fgg89/docker-ap