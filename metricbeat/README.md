# Metricbeat container for CoreELEC ARM64

## What does the service actually do?

Lightweight shipper for metrics
Collect metrics from your systems and services. From CPU to memory, Redis to NGINX, and much more, Metricbeat is a lightweight way to send system and service statistics.

[https://www.elastic.co/beats/metricbeat](https://www.elastic.co/beats/metricbeat)

## Usage:

```bash
git clone https://github.com/tamusiunas/coreelec-docker-containers.git
cd coreelec-docker-containers/metricbeat

#
# Important! Create the structure to persist data before starting the containers.
#
# Create the structure under /storage/.docker/volumes/elk/
cp -a storage/. /storage

#
# This container comes configured to send docker metrics to ElasticSearch, setup dashboards (load them into Kibana) and monitor the service.
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
