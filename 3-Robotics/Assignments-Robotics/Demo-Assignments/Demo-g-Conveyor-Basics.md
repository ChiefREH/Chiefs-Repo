# CONVEYOR BASICS

- Make a dummy Simulation Editor program to get into Cycle Start mode, so the animation works.
- Adding a Conveyor to the World: Right-click Machines > Add Machine > CAD Library > Fixtures


## MOTION CONTROL TYPE
- Select "Device IO Controlled"

## AXIS TYPE
- Rotary moves around the Axis selected
- Linear moves in line with the Axis selected

## SPEED
- Top Speed option is how fast the package moves away from the starting point
- Bottom Speed option is how fast the package returns to the starting point
    - We’ll set this to 100,000 so it snaps back really fast

## INPUTS/OUTPUTS
- Think of this as a PLC built into the conveyor
- This IO can interface with the Robot IO without using Cell Interconnect

### Inputs (top)
- When the Controller listed in “Output Dev” activates the “IO Tag” with “Value,” the Conveyor will then move the package to the “Location” indicated at the SPEED set above.
- This section receives signal from the Robot IO.

> Example read left to right: When Robot Controller 1 turns Digital Output DO[3] to ON, move the Box 950mm away from the starting position at 250mm/sec.

### Outputs (bottom)
- When the package arrives at the “Location” indicated, the conveyor will signal the Controller listed in “Input Dev” at the “IO Tag” with the “Value” indicated.
- This section sends signal to the Robot IO.
    - This is a good way to set the timing of robot motion without relying on timers.

> Example read right to left: When the Box arrives at the location 50mm from the starting position, send an OFF signal to the Robot Controller 1 Digital Input DI[3].

## VIDEO REFERENCE

- Conveyor Basics
- Conveyor Table Pick & Place
