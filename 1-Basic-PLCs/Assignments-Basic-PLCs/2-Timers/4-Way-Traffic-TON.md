# 4-Way Traffic (N-S-E-W) TON Timers

Emulate a 4-way NORTH-SOUTH-EAST-WEST traffic pattern using the following LD instructions:
- All necessary XIC and XIO instructions 
- (3) TON Timers to control the NORTH-SOUTH lights 
- (3) TON Timers to control the EAST-WEST lights 
- (6) OTE instructions to serve as the “traffic lights”

## TIMING
- All Red Lights = 10 seconds 
- All Green Lights = 7 seconds 
- All Yellow Lights = 3 seconds 

## PARAMETERS

- Use a SEAL-IN circuit to start/stop the routine 
- Once started, the routine must continually loop 
- The light sequence must follow the common logical sequence 
- Do not create a traffic jam or motor vehicle accident!

### Do NOT create a traffic jam!

*Proper rung documentation is mandatory.