# MIDTERM LAB PROJECT

## ROBOT WAVE OVER WIFI

- Reconfigure the RPis to operate on WiFi only
- Utilize the Node-Red dashboard UI for the interface
- Trigger the robotic sequence using a cellphone

### Group Exercise

- Create a program that produces a "wave" effect with the lab robots.
- Utilize MQTT and RPis to coordinate signals between individual robots.
- The central RPi will be used to initiate the wave sequence.
- All robots will need to be in the same Ready Position before execution.
- The sequence will include all robots (in order).
- The robots will execute their code once before signaling the next robot.
- The last robot will signal the central RPi when its routine is finished.
- The central RPi must be able to run the sequence multiple times without error.


## ADVANCED CONFIG

- All robots will have a **Safe Position** that can be triggered from the central RPi.
    - _A Safe Pos is one that is away from the work area._

