# SEQUENCER OUTPUT TRAFFIC

Replicate a N-S-E-W traffic pattern using the SQO instruction.

- _See the Traffic Light Outputs file in the Homebrew folder for emulated and hardware LED format._

## WORK ORDER:
Create this traffic routine (with proper timing) using the following instructions:
- (1) TON instruction
- (1) SQO instruction with an array of DINT[5] 
- MOV instructions as needed
    - _for the TON.PRE ?_
- Math instructions as needed
- Comparison instructions as needed
    - _for the TON.PRE ?_
- All necessary XIC and XIO instructions 

## NOTE:

- OTE instructions for LIGHTS are limited to lab only (_see "poor man's array"_)
    - _Using branched light OTEs defeats the purpose of the SQO instruction_


## TIMING:
Routine must follow the common logical sequence (Red, Green, Yellow):
- Red Lights - 10 seconds 
- Green Lights - 7 seconds 
- Yellow Lights - 3 seconds 

DO NOT CAUSE A TRAFFIC JAM OR COLLISION!

## PARAMETERS:
- Routine must operate with a SEAL-IN CIRCUIT. 
- Once started, the routine must run in a continuous loop. 
- Properly configured I/O Modules (emulated and lab) are required.
- Proper documentation and rung comments are mandatory.
- Lab safety is non-negotiable.
