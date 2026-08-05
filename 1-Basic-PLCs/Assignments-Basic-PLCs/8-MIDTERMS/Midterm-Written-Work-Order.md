# LJ's WRITTEN WORK ORDER

## PLC Program Test

Create a PLC program for the startup and stop of a motor with its oil pump and fan. There are 2 inputs called **“Start_PB”** and **“Stop_PB”**. The initial state remains with the motor off. There are 4 motor speeds (25%, 50%, 75% and 100%).

After pressing the Start button the motor, fan and oil pump will turn on. The motor will start running at 25%. Then, it will move to the next speed every 5 seconds until it finally remains running at 100%. The motor should stop anytime the Stop button is pressed, regardless of the speed.

- If the motor has operated for less than 20 seconds, the oil pump should go off when the motor is turned off, and the fan should run for an additional 5 seconds after the motor is shut down.

- If the motor has operated for more than 20s, the oil pump should remain on for 20 seconds when the motor is turned off, and then the fan should run for an additional 15 seconds after the motor is shut down.

There are 2 lights (**“Green_Light”** and **“Yellow_light”**). The green light will be on while the motor is running. The yellow light will be on while the motor is stopped.

Use a counter to count the times that push start has been pressed. When the counter reaches 10, turn on a bit called **“SERVICE”**. Use a push button input called **“RESET”** to reset the count and turn off the **“SERVICE”** bit.

## EXAMPLE

```text
+----------------------------------------------------------------------------------------+
|      +------------------+    +----------------------+      +--------------------+      |
|      | INPUTS           |    |                      |      | OUTPUTS            |      |
|      |                  |    |                      |      |                    |      |
|      | START_PB         |----|                      |------| GREEN_LIGHT        |      |
|      |                  |    |                      |------| YELLOW_LIGHT       |      |
|      | STOP_PB          |----|         PLC          |------| M1_25              |      |
|      |                  |    |                      |------| M1_50              |      |
|      | RESET            |----|                      |------| M1_75              |      |
|      |                  |    |                      |------| M1_100             |      |
|      |                  |    |                      |------| OIL_PUMP           |      |
|      +------------------+    |                      |------| FAN                |      |
|                              +----------------------+      +--------------------+      |
+----------------------------------------------------------------------------------------+
```