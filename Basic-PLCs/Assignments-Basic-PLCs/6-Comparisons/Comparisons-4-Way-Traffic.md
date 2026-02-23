# COMPARISON INSTRUCTIONS FOR N-S/E-W TRAFFIC

Create an EMULATED and LAB routine for North-South-East-West traffic lights using only these instructions.

## NORTH-SOUTH INSTRUCTIONS:

Use any combination of these COMPARISON instructions to properly control the N-S lights: 
- GEQ instructions (as needed)
- LES instructions (as needed)
- GRT instructions (as needed)
- LEQ instructions (as needed)
- EQU instructions (as needed)

No other Comparison instructions are required.

- ONS instructions (as needed)
- OTE instructions must be properly tagged, grouped, branched and ALIASED to an I/O module 


## EAST-WEST INSTRUCTIONS:

Use (3) LIM instructions to properly control the E-W lights.

- ONS instructions (as needed)
- OTE instructions must be properly tagged, grouped, branched and ALIASED to an I/O module

No other instructions are required.


## PARAMETERS:

- Only (1) TON with a 20 second .PRE can be used. 
    - All RED lights: 10 seconds 
    - All YELLOW lights: 3 seconds 
    - All GREEN lights: 7 seconds

XIC and XIO are only used for controlling the TON timer, not the lights.


## NOTES:

- Use a SEAL-IN circuit to start/stop the routine 
- Once started, the routine must continually loop 
- The light sequence must follow the common logical sequence 
- Do not create a traffic jam or motor vehicle accident! 



*Proper rung documentation is mandatory.

>_Refer to Traffic LED Outputs in the Basic PLC Homebrew Rules for number of OTEs and arrangement._

