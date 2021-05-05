# Journalbeat container for CoreELEC ARM64

## What does the service actually do?

Journalbeat is a lightweight shipper for forwarding and centralizing log data from systemd journals.

[https://www.elastic.co/guide/en/beats/journalbeat/current/journalbeat-overview.html](https://www.elastic.co/guide/en/beats/journalbeat/current/journalbeat-overview.html)

## Usage:

```bash
git clone https://github.com/tamusiunas/coreelec-docker-containers.git
cd coreelec-docker-containers/journalbeat

#
# Important! Create the structure to persist data before starting the containers.
#
# Create the structure under /storage/.docker/volumes/elk/
cp -a storage/. /storage

#
# This container comes configured to send docker journals to ElasticSearch and monitor the service.
#

#
# Add Kibana host, ElasticSearch host and user/password editing the file docker-compose.yml
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
