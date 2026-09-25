# EMULATE + CONVERT 4-Way TOF + CTD

1. Emulate in the classroom
2. Convert for use in the lab

A 4-way **NORTH-SOUTH/EAST-WEST** traffic pattern using the following LD instructions:
- All necessary XIC,XIO and OTE instructions
- (3) TOF Timers to control the NORTH-SOUTH lights 
- (3) TOF Timers to control the EAST-WEST lights 
- (1) CTD Counter to control the number of program loops
- (1) RES Reset instruction to **manually** reset the CTD from software
> The RES does not require an additional button.


## TIMING
- All Red Lights = 10 seconds 
- All Green Lights = 7 seconds 
- All Yellow Lights = 3 seconds
- Counter = 3 loops



## PARAMETERS

- Use a SEAL-IN circuit to start/stop the routine
    - Must use wired push-buttons in the lab
- Routine must continually loop until the Counter is done
- When the Counter is done, the routine must shutdown on its own
    - _Operator must manually toggle the RES on/off to reset the CTD **before** restarting the program_
- The light sequence must follow the common logical sequence 
- Do not create a traffic jam or motor vehicle accident!


*Proper rung documentation is mandatory.