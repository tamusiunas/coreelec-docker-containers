# Heartbeat container for CoreELEC ARM64

## What does the service actually do?

Lightweight shipper for uptime monitoring

Monitor services for their availability with active probing. Given a list of URLs, Heartbeat asks the simple question: Are you alive? Heartbeat ships this information and response time to the rest of the Elastic Stack for further analysis.

[https://www.elastic.co/beats/heartbeat](https://www.elastic.co/beats/heartbeat)

## Usage:

```bash
git clone https://github.com/tamusiunas/coreelec-docker-containers.git
cd coreelec-docker-containers/heartbeat

#
# Important! Create the structure to persist data before starting the containers.
#
# Create the structure under /storage/.docker/volumes
cp -a storage/. /storage

#
# Edit /storage/.docker/volumes/heartbeat/heartbeat.yml and configure hosts to monitor HTTP, ICMP and TCP
# (there are two examples for HTTP and ICMP)
#

#
# Edit docker-compose.yml and add Kibana host, ElasticSearch host and user/password
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
