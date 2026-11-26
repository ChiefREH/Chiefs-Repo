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

- A full loop means all Cylinders extended once and retracted once.
- When Counter = 3 loops, stop all cylinders, all lights out
- When counter is reset to 0, sequence begins again

## DESIGN NOTES

- Control Valves PILOT PRESSURE CONTROL, not ELECTRICAL SOLENOID CONTROL
- Lights are ELECTRICAL CONTROL
- Counter is an ELECTRICAL CONTROLS component

>The trick is figuring out how to interface the electrical with the pressure
