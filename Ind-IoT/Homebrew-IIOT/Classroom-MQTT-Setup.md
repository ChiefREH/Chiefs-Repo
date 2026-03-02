# BASIC MQTT PARAMETERS

## Mosquitto from the CLI

- _mosquitto_sub -h (host) -p (port) -t (topic)_
- _mosquitto_pub -h (host) -t (topic) -m (message)_

## MQTT In / MQTT Out Nodes
### REMEMBER: YOU CANNOT USE LOCALHOST AS SERVER
- Must use **host.docker.internal:1883** when in Docker Desktop
- WINDOWS: Might require full path to the mosquitto_pub/sub

