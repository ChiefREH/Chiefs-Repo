# Indirect Move FROM an Array + GSV capture

Create a routine that will pull a number **FROM** an Array and move the data to an Output module using the following instructions:

- All necessary XIC and XIO instructions 
- TON instruction(s) as needed 
- CTU instruction(s) as needed 
- DINT[16] Array to store the static numbers 
- ONS instruction(s) as needed 
- GSV instruction 
    - Starting Date/Time only, not continuously 
- DINT[7] Array to store the captured GSV data 
- MOV instruction(s) as needed 
- CLR instruction(s) as needed 
- RES instruction(s) as needed 
- BRANCHES as needed 

## STATIC NUMBERS TO PULL FROM ARRAY STORAGE
- 1, 2, 4, 8, 16, 32, 64, 128, 256, 512, 1024, 2048, 4096, 8192, 16384, 32768

## TIMING
- TON .PRE = 1 second 
- CTU .PRE = 16 

## PARAMETERS
- Use a "seal-in" circuit to start/stop the routine.
- Once running, the routine must run continuously.
- All Array elements must be moved in order, from the first element to the last element. 
- When the last element is moved, the index must reset before faulting the controller. 
- Any values moved to the Output Module must be presented in the BINARY style radix. 
- If stop/restart, must CLR the output tag to begin again at all 0s.

*Proper rung documentation is mandatory.