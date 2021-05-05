# eclipse-mosquitto container for CoreELEC ARM64

## What does the service actually do?

Eclipse Mosquitto is an open source (EPL/EDL licensed) message broker that implements the MQTT protocol versions 5.0, 3.1.1 and 3.1. Mosquitto is lightweight and is suitable for use on all devices from low power single board computers to full servers.

**Based on [https://hub.docker.com/_/eclipse-mosquitto](https://hub.docker.com/_/eclipse-mosquitto)**

[https://mosquitto.org](https://mosquitto.org)

## Usage:

```bash
git clone https://github.com/tamusiunas/coreelec-docker-containers.git
cd coreelec-docker-containers/eclipse-mosquitto

# Create the structure under /storage/.docker/volumes/mosquitto
mkdir -p /storage/.docker/volumes/mosquitto/data
mkdir -p /storage/.docker/volumes/mosquitto/log
mkdir -p /storage/.docker/volumes/mosquitto/config

# Adjust permissions
chown -R 1883:1883 /storage/.docker/volumes/mosquitto/data
chown -R 1883:1883 /storage/.docker/volumes/mosquitto/log
chown -R 1883:1883 /storage/.docker/volumes/mosquitto/config

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
1883 | 1883 | TCP
8883 | 8883 | TCP

For more information about docker with CoreELEC see [docker-coreelec project](https://github.com/tamusiunas/docker-coreelec).
