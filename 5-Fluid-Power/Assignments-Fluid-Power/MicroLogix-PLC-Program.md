# MicroLogix PLC PROGRAM (TRAFFIC)

Create the following PLC program using MicroLogix EMULATION:

## NORTH-SOUTH / EAST-WEST TRAFFIC

- (3) TON timers for N-S traffic lights
- (3) TON timers for E-W traffic lights
- (6) OTE outputs (one for each light)
    - Properly addressed and branched
- (1) CTU counter to track number of loops
- All necessary XIO and XIC instructions
- Any RES reset instructions, as needed


## PARAMETERS:

- Standard Light Interval:
    - RED lights: 10 seconds 
    - YELLOW lights: 3 seconds 
    - GREEN lights: 7 seconds
- Loop Counters:
    - Count for **3 loops**


## NOTES:

- Use a simple SEAL-IN circuit to start/stop the routine
- The light sequence must follow the common logical sequence 
- Do not create a traffic jam or motor vehicle accident!
- Once activated, the routine must run continuously until the counter is done.
- When the counter is done, the routine must shut itself off automatically


*Proper rung documentation is mandatory.

>_Refer to Traffic LED Outputs in the Basic PLC Homebrew Rules for number of OTEs and arrangement._
