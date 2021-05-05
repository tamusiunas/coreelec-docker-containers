# duckdns container for CoreELEC ARM64

## What does the service actually do?

Duck DNS is a free service which will point a DNS (sub domains of duckdns.org) to an IP of your choice

**Based on [https://github.com/linuxserver/docker-duckdns](https://github.com/linuxserver/docker-duckdns)**

[https://www.duckdns.org](https://www.duckdns.org)

- Before configure the service pick a token at [https://www.duckdns.org](https://www.duckdns.org)

## Usage:

```bash
git clone https://github.com/tamusiunas/coreelec-docker-containers.git
cd coreelec-docker-containers/duckdns

#
# Important! Edit file docker-compose.yml and enter yout domain and token previously got.
#

#
# Containers usage
#
docker-compose create # (Create services)
docker-compose up # (Create and start containers - in foreground)
docker-compose down # (Stop and remove resources)
docker-compose start # (Start services - in background)
docker-compose stop # (Stop services)

```

For more information about docker with CoreELEC see [docker-coreelec project](https://github.com/tamusiunas/docker-coreelec).
