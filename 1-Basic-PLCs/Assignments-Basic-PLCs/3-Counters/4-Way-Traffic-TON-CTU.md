# 4-Way TON + CTU

Emulate a 4-way **NORTH-SOUTH-EAST-WEST** traffic pattern using the following LD instructions:
- All necessary XIC and XIO instructions 
- (3) TON Timers to control the NORTH-SOUTH lights 
- (3) TON Timers to control the EAST-WEST lights 
- (6) OTE instructions to serve as the “traffic lights”
- (1) CTU Counter to control the number of program loops
- (1) RES Reset instruction to **manually** reset the CTU

## TIMING
- All Red Lights = 10 seconds 
- All Green Lights = 7 seconds 
- All Yellow Lights = 3 seconds
- Counter = 3 loops

## PARAMETERS

- Use a SEAL-IN circuit to start/stop the routine 
- Routine must continually loop until the Counter is done
- When the Counter is done, the routine must shutdown on its own
    - _Operator must manually toggle the RES on/off to reset the CTU **before** restarting the program_
- The light sequence must follow the common logical sequence 
- Do not create a traffic jam or motor vehicle accident!


*Proper rung documentation is mandatory.