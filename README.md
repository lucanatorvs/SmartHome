# My custom smart home deploymant

Running on a raspberry pi, this is a custom smart home deployment using the [Home Assistant](https://home-assistant.io/) framework.

## Installation

You need a .env file with the following variables:

```
variables yet to be added
.env file not functional yet
```

All the running docker containers should be:

- [x] [HomeAssistant](https://hub.docker.com/r/homeassistant/home-assistant) is integrated into the docker compose file
- [x] [Influxdb](https://hub.docker.com/_/influxdb) is integrated into the docker compose file
- [x] [Grafana](https://hub.docker.com/r/grafana/grafana) is integrated into the docker compose file
- [x] [Mosquitto](https://hub.docker.com/_/eclipse-mosquitto) is integrated into the docker compose file
- [ ] [Speedtest](https://hub.docker.com/r/robinmanuelthiel/speedtest) is integrated into the docker compose file
- [ ] [Zigbee2mqtt](https://hub.docker.com/r/koenkk/zigbee2mqtt) is integrated into the docker compose file
- [x] [Node-Red](https://hub.docker.com/r/nodered/node-red) is integrated into the docker compose file
- [ ] [mqtt-bridge](mqtt2influxdb_bridge/Dockerfile) is integrated into the docker compose file
- [x] [Portainer](https://hub.docker.com/r/portainer/portainer-ce) is integrated into the docker compose file

## Usage

```bash
docker-compose up # starts the containers
docker-compose down # stops the containers
```

## Todo

- [x] Create a docker compose file to deploy the home assistant instance and other components, such as a mqtt broker, Influxdb databace, Grafana and node-red
- [ ] add to the docker compose file to deploy the Zigbee2mqtt functionality
- [ ] Intigrate it with ikea TRÅDFRI lights and sensors, using the above mentiond Zigbee CC2531 usb dongle
- [ ] Create custom sensors and lights to be controlled by the home assistant instance
- [ ] Create custom controll scripts to make my home work for me

## What is not working / What needs to be fixt first (ToDo)

- [ ] Zigbee CC2531 usb dongle needs to be flashed with the firmware