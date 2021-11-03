---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
maintitle: Build a Cloud
title: Build a Cloud
sortOrder: 4
permalink: /cloud/
breadcrumb:
    - 
      name: Build a cloud
---

*AirMeter.io* provides data logging and charting on device this should generally be accompanied with publishing to "the cloud" on a periodic basis. Readings from the sensors are published to remote servers using the industry standard protocol MQTT.

There are several services which are either free or will at a minimal monthly cost provide MQTT hosting with dashboards. If the devices being monitored have strong internet connectivity this can be the easiest option. This option can have privacy issues be sure to consult your chosen service's policies carefully.

It is also however relatively simple to build your own "personal cloud" either using AWS, Azure etc or by hosting a server the local the network. For small scale such as a home a Raspberry Pi4 or similar is more than sufficient for this task.

Later detailed instructions will be included. For now here is a basic set of open source components which can form a private "cloud" with MQTT and basic dashboards.
- [Eclipse Mosquitto](https://mosquitto.org/) - Eclipse Mosquitto is an open source MQTT server which *AirMeter.io* can publish readings to.
- [InfluxDB](https://github.com/influxdata/influxdb) - InfluxDB is an open source time series database to store readings published over MQTT.
- [Telegraf](https://github.com/influxdata/telegraf) - Telegraf is to connect InfluxDB to the Eclipse Mosquitto server.
- [Grafana](https://github.com/grafana/grafana) - Grafana as a dashboarding solution to visualise the data stored in the InfluxDB in drill down charts.



