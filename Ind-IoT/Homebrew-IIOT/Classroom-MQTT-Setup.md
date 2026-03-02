# BASIC MQTT PARAMETERS

## Mosquitto from the CLI

- _mosquitto_sub -h (host) -p (port) -t (topic)_
- _mosquitto_pub -h (host) -t (topic) -m (message)_

## MQTT In / MQTT Out Nodes
### REMEMBER: YOU CANNOT USE LOCALHOST AS SERVER
- Must use **host.docker.internal:1883** when in Docker Desktop
- WINDOWS might require full path to the mosquitto_pub/sub

### Example

_C:\Program Files\mosquitto\mosquitto_publish.exe -h 192.168.1.15 -p 1880 -t test/status -m "Hello, World"_