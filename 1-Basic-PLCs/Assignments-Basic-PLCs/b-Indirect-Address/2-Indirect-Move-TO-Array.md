# Indirect Move TO an Array with RTO as RNG

Create a routine that will move a variable number into Array elements sequentially, using the following instructions:
- All necessary XIC and XIO instructions 
- 1 TON instruction as a pulse timer 
- 1 RTO instruction as the variable number source 
- 1 CTU instruction as the indirect index 
- 1 DINT[10] Array to store the variable numbers 
- MOV instruction(s) as needed
- COP instruction(s) as needed
- RES instruction(s) as needed
- CLR instruction(s) as needed

## TIMING
- TON .PRE = 1 second 
- RTO .PRE = 32,767 seconds 
- CTU .PRE = 10 

## PARAMETERS
- Use a "seal-in" circuit to start/stop the routine
- Once running, the routine must run continuously
- All Array elements must be filled in sequence, from the **first** element to the **last** element. 
- When the last element is filled, the index must reset **before** faulting the controller. 
- New variables will overwrite the old variables, starting again at the first element. 
- On stop/restart, the output tag must revert to all zeroes.
    - The index position must restart at zero.

*Proper rung documentation is mandatory.