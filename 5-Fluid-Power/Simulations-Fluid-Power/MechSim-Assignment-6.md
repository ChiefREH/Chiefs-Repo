# MECHSIMULATOR ASSIGNMENT 6

Using a mix of CONTROLS, create the following simulation:

- Extend Cylinder 1 / Red light ON
- Wait
- Extend Cylinder 2 / Yellow light ON
- Wait
- Extend Cylinder 3 / Green light ON
- Wait
- Retract Cylinder 3 / Green light OFF
- Wait
- Retract Cylinder 2 / Yellow light OFF
- Wait
- Retract Cylinder 1 / Red light OFF
- Wait
- Cycle Counter + 1
- Repeat

## PARAMETERS

- A full loop means all Cylinders extended onces and retracted once.
- When Counter = 3 loops, stop all cylinders, all lights out
- Reset to 0, sequence begins again
- Counter should only increase when Cylinder 1 if fully RETRACTED / Red light OFF
