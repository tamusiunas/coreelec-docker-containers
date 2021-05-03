# homebridge container for CoreELEC ARM64

## What does the service actually do?

Homebridge allows you to integrate with smart home devices that do not natively support HomeKit. There are over 2,000 Homebridge plugins supporting thousands of different smart accessories.

**Based on [https://github.com/oznu/docker-homebridge](https://github.com/oznu/docker-homebridge)**

[https://www.duckdns.org](https://www.duckdns.org)

## Usage:

```bash
git clone https://github.com/tamusiunas/coreelec-docker-containers.git
cd homebridge

#
# Important! Create the structure to persist data before starting the container.
#
mkdir -p /storage/.docker/volumes/homebridge

#
# Container usage
#
docker-compose up # (run in foreground)
docker-compose down # (remove container)
docker-compose start # (run on background)
docker-compose start # (stop service)

```

For more information about docker with CoreELEC see [docker-coreelec project](https://github.com/tamusiunas/docker-coreelec).