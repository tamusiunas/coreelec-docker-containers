ARG ELK_VERSION

# https://www.docker.elastic.co/
FROM tamusiunas/logstash:${ELK_VERSION}

# Add your logstash plugins setup here
# Example: RUN logstash-plugin install logstash-filter-json
RUN logstash-plugin install logstash-input-syslog
RUN logstash-plugin install logstash-input-snmp
