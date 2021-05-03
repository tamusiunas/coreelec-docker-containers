# ELK Stack container for CoreELEC ARM64

## What does the service actually do?

"ELK" is the acronym for three open source projects: Elasticsearch, Logstash, and Kibana. Elasticsearch is a search and analytics engine. Logstash is a server‑side data processing pipeline that ingests data from multiple sources simultaneously, transforms it, and then sends it to a "stash" like Elasticsearch. Kibana lets users visualize data with charts and graphs in Elasticsearch.
The Elastic Stack is the next evolution of the ELK Stack.

[https://www.elastic.co/what-is/elk-stack](https://www.elastic.co/what-is/elk-stack)

## Usage:

```bash
git clone https://github.com/tamusiunas/coreelec-docker-containers.git
cd coreelec-docker-containers/elk

#
# Important! Create the structure to persist data before starting the containers.
#

# Create the structure under /storage/.docker/volumes/elk/
cp -a storage /storage

# Adjust permissions
chown -R 1000:1000 /storage/.docker/volumes/elk

#
# The default username/password is elastic/changeme
# To change the default password edit the files docker-compose.yml and /storage/.docker/volumes/elk/logstash/pipelines/pipeline_1.conf
# If you changed the password inside Kibana, edit the file /storage/.docker/volumes/elk/logstash/pipelines/pipeline_1.conf and update it
#

#
# Containers usage
#
docker-compose up # (run in foreground)
docker-compose down # (remove container)
docker-compose start # (run on background)
docker-compose start # (stop service)

```

It's recommended to use a 4GB RAM model to run ELK (ELK uses about 1.5GB RAM) and a fast SD-Card to store the data. 

For more information about docker with CoreELEC see [docker-coreelec project](https://github.com/tamusiunas/docker-coreelec).