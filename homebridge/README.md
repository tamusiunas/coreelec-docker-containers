# homebridge container for CoreELEC ARM64

## What does the service actually do?

Homebridge allows you to integrate with smart home devices that do not natively support HomeKit. There are over 2,000 Homebridge plugins supporting thousands of different smart accessories.

**Based on [https://github.com/oznu/docker-homebridge](https://github.com/oznu/docker-homebridge)**

[https://www.duckdns.org](https://www.duckdns.org)

## Usage:

```bash
git clone https://github.com/tamusiunas/coreelec-docker-containers.git
cd coreelec-docker-containers/homebridge

#
# Important! Create the structure to persist data before starting the container.
#
mkdir -p /storage/.docker/volumes/homebridge

#
# Containers usage
#
docker-compose create # (Create services)
docker-compose up # (Create and start containers - in foreground)
docker-compose down # (Stop and remove resources)
docker-compose start # (Start services - in background)
docker-compose stop # (Stop services)

```

Ports mapped to host

Host | Container | Prtocol 
-----|-----------|--------
8581 | 8581      | TCP

For more information about docker with CoreELEC see [docker-coreelec project](https://github.com/tamusiunas/docker-coreelec).
