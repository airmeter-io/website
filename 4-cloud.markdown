---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
maintitle: Build a Cloud
sortOrder: 4
permalink: /cloud/
breadcrumb:
    - 
      name: Build a cloud
---

Whilst *AirMeter.io* provides data logging and charting on device this should generally be complimented with publishing data to "the cloud" on a periodic basis. Readings from the sensors are published to remote servers in "the cloud" using the industry standard protocol MQTT.

There are several services which either for free or minimal monthly cost provide MQTT hosting with dashboards. If all the devices being monitored have reliable internet connectivity & privacy isn't a huge concern this can be the easiest option.

It is also however relatively simple to build your own "personal cloud" either using AWS, Azure etc or by just hosting a server on the network to which the *AirMeter.io* monitor devices are connected. For small scale such as a home a Raspberry Pi4 or similar is more than sufficient.

Later this page will be expanded to include detailed instructions. But for now here is a set of components which can be used to build a private "cloud" with MQTT and basic dashboard functionality.
- [Eclipse Mosquitto](https://mosquitto.org/) - Eclipse Mosquitto an open source MQTT server to which *AirMeter.io* can publish readings.
- [InfluxDB](https://github.com/influxdata/influxdb) - InfluxDB is an open source time series database in which to store readings published using MQTT.
- [Telegraf](https://github.com/influxdata/telegraf) - Telegraf is used to connect InfluxDB to the Eclipse Mosquitto server.
- [Grafana](https://github.com/grafana/grafana) - Grafana is a dashboarding solution that enables the data stored in the InfluxDB to be displayed in a visual & drill down form.



