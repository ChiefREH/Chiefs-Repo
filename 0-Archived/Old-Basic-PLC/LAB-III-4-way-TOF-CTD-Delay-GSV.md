# 4-way TOF + CTD + TOF delay + GSV capture

Create a LAB routine for North-South/East-West traffic lights using TOF and CTD instructions.


## PARAMETERS:

- Standard Light Interval:
    - RED lights: 10 seconds 
    - YELLOW lights: 3 seconds 
    - GREEN lights: 7 seconds
- Loop Counter:
    - Count for **3 loops**
- Delay Timer:
    - Delay automatic restart for **6 seconds**
- GSV to capture the starting WallClockTime

## NOTES:

- Use a SEAL-IN circuit to start/stop the routine
- The light sequence must follow the common logical sequence 
    - Do not create a traffic jam or motor vehicle accident!
- Once activated, the routine must run continuously until the counter is done.
- When the counter is done, the routine must delay before restarting automatically.
- WallClockTime capture is for the starting DateTime only, not continuously.

*Proper rung documentation is mandatory.

>_Refer to Traffic LED Outputs in the Basic PLC Homebrew Rules for number of OTEs and arrangement._
