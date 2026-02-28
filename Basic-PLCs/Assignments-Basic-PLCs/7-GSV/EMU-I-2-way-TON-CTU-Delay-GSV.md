# 2-way TON + CTU + TON delay + GSV capture

Create an EMULATED routine for North-South traffic lights using these instructions.

## NORTH-SOUTH TRAFFIC

- (3) TON timers for N-S traffic lights
- (1) CTU counter to track the number of loops
- (1) TON timer to act as a delay timer
- (1) GSV to capture the starting WallClockTime
- All necessary XIO, XIC and ONS instructions
- All necessary OTE instructions
    - Properly tagged, aliased, grouped and branched
- Any RES reset instructions, as needed


## PARAMETERS:

- Standard Light Interval:
    - RED lights: 10 seconds 
    - YELLOW lights: 3 seconds 
    - GREEN lights: 7 seconds
- Loop Counter:
    - Count for **3 loops**
- Delay Timer:
    - Delay automatic restart for **6 seconds**


## NOTES:

- Use a SEAL-IN circuit to start/stop the routine
- The light sequence must follow the common logical sequence 
- Do not create a traffic jam or motor vehicle accident!
- Once activated, the routine must run continuously until the counter is done.
- When the counter is done, the routine must delay before restarting automatically.
- WallClockTime capture is for the starting DateTime only, not continuously.



*Proper rung documentation is mandatory.

>_Refer to Traffic LED Outputs in the Basic PLC Homebrew Rules for number of OTEs and arrangement._