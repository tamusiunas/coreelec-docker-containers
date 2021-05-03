# corelec-docker-containers

**Docker Containers for CoreELEC**

CoreELEC is a Linux system (JeOS - Just enough Operational System) that runs on devices with Amlogic processors. It has the minimum required to run the Kodi system and uses the original Amlogic Kernel for Android (4.9.113) having support for almost all embedded devices (Bluetooth, WiFi, Ethernet, Audio and Video Output, Hardware Video Decoding) using the original Android structure while other Linux distributions often do not support all installed devices.

Usually new software is installed through add-on using the GUI interface (Kodi), where the software is usually aimed for multimedia activities. One exception is the system-oriented software Docker, however it is limited to version 19.

Generally boxes sold with the Amlogic processors line have reasonably high memory for this type of system (4/8 GB) and multi-core processor with a very attractive price. The possibility of using a docker, especially the latest versions with security fixes, can make this type of equipment very efficient for a lot of domestic applications, such as servers for IoT.

**This project provides containers to run on ARM64 distro**

##List of Containers

Container|Description|Site
---------|-----------|----
[duckdns](tree/main/duckdns)|Free dynamic DNS hosted on AWS| [duckdns.org](https://www.duckdns.org)
[eclipse-mosquitto](tree/main/eclipse-mosquitto)|Message broker that implements the MQTT protocol|[mosquitto.org](https://mosquitto.org)
[elk](tree/main/elk)|Elasticsearch, Logstash, and Kibana|[elastic.co](https://www.elastic.co/what-is/elk-stack)
[homebridge](tree/main/homebridge)|Integrate smart home devices that do not natively support HomeKit|[homebridge.io](https://homebridge.io)
[metricbeat](tree/main/metricbeat)|System-level monitoring|[elastic.co](https://www.elastic.co/beats/metricbeat)