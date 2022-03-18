# My custom smart home deploymant

Running on a raspberry pi, this is a custom smart home deployment using the [Home Assistant](https://home-assistant.io/) framework.

## Installation

you need a .env file with the following variables:


running codker containers chould be:

- [HomeAssistant](https://hub.docker.com/r/homeassistant/home-assistant)
- [Influxdb](https://hub.docker.com/_/influxdb)
- [Grafana](https://hub.docker.com/r/grafana/grafana)
- [Mosquitto](https://hub.docker.com/_/eclipse-mosquitto)
- [Speedtest](https://hub.docker.com/r/robinmanuelthiel/speedtest)
- [Zigbee2mqtt](https://hub.docker.com/r/koenkk/zigbee2mqtt)
- [Node-Red](https://hub.docker.com/r/nodered/node-red)
- mqtt-bridge, see docker file 
- [Portainer](https://hub.docker.com/r/portainer/portainer-ce)

## todo

- Create a docker compose file to deploy the home assistant instance and other components, such as a mqtt broker, Influxdb databace, Grafana and node-red.
- intigrate it with ikea TRÅDFRI lights and sensors, using a Zigbee CC2531 usb dongle.
- create custom sensors and lights to be controlled by the home assistant instance.
- create custom controll scripts to make my home work for me.