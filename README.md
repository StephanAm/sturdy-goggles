# sturdy-goggles

## Intro
The basic idea here is to quickly get a home automation server up and running. Mostly to document the set-up that I'm using.

## Components
### Mosquitto
Listening on default port 1883. (and port exposed as-is from container)
Other containers should reference using host:mqtt port:1883

### Node-Red
Listening on default port 1880. (and port exposed as-is from container)
Also slipstreamed with node-red-dashboard and some other useful UI intruments.

### Home Assistant
Listening on default port 8123. (and port exposed as-is from container)

### Nginx
Listening on port 80.
hosts a index page on /
redirects /nodered/ to nodered:1880/
redirects /dash/ to nodered:1880/ui
redirects /homeassistant/ to homeassistant:8123/
