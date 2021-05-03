# duckdns container for CoreELEC ARM64

## What does the service actually do?

Duck DNS is a free service which will point a DNS (sub domains of duckdns.org) to an IP of your choice

**Based on [https://github.com/linuxserver/docker-duckdns](https://github.com/linuxserver/docker-duckdns)**

[https://www.duckdns.org](https://www.duckdns.org)

## Usage:

```bash
#
# Important! Edit file docker-compose.yml and enter yout domain and token previously got at [https://www.duckdns.org](https://www.duckdns.org).
#

#
# Container usage
#
docker-compose up (run in foreground)
docker-compose down (remove container)
docker-compose start (run on background)
docker-compose start (stop service)

```

For more information about docker with CoreELEC see [docker-coreelec project](https://github.com/tamusiunas/docker-coreelec).