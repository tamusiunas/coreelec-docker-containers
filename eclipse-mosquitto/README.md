# eclipse-mosquitto container for CoreELEC ARM64

## What does the service actually do?

Eclipse Mosquitto is an open source (EPL/EDL licensed) message broker that implements the MQTT protocol versions 5.0, 3.1.1 and 3.1. Mosquitto is lightweight and is suitable for use on all devices from low power single board computers to full servers.

**Based on [https://hub.docker.com/_/eclipse-mosquitto](https://hub.docker.com/_/eclipse-mosquitto)**

[https://mosquitto.org](https://mosquitto.org)

## Usage:

```bash
#
# Container usage
#
docker-compose up (run in foreground)
docker-compose down (remove container)
docker-compose start (run on background)
docker-compose start (stop service)

```

For more information about docker with CoreELEC see [docker-coreelec project](https://github.com/tamusiunas/docker-coreelec).