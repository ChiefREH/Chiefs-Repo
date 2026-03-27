# ESP32 + SENSOR INTEGRATION

- Install and wire ESP32 for power
- Install and wire sensors
- Make all necessary network connections (wlan0)
    - _see the Static IP notes in Homebrew_

## Sketch 1

- Code to push an MQTT message when each sensor is triggered
    - Central Hub will display this information on the monitor

## Sketch 2

- Code to operate the conveyor motor relay via MQTT messages/Node-Red
    - Run each motor for 5 seconds, then stop
- Modify the User Pushbutton to act as an emergency stop only (no toggle)
