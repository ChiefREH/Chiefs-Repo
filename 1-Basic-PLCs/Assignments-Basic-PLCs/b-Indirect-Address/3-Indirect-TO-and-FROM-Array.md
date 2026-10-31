# EMU + LAB: Indirect Move TO and FROM an Array + GSV capture

- Create a routine that will move numbers TO and FROM and Array
- Include properly configured output module (emulated and lab)
- Capture Date/Time data on start (not continuously)

## OPERATIONAL SEQUENCE
1. Move a random variable **TO** the storage DINT[10]  Array, in sequential order. 
2. When the Array is full, stop sending variables. 
3. Pull a variable **FROM** the storage DINT[10] Array and move it to an output module, in sequential order. 
4. When the last variable is pulled and moved, go to Step #1 and repeat.

## TIMING
- TON .PRE = 1 second 
- RTO .PRE = 32767 seconds 
- CTU .PRE = 10 

## PARAMETERS
- Use a "seal-in" circuit to start/stop the routine
    - Alias the seal-in to buttons in the Lab
- Once running, the routine must operate continuously
- All Array elements must be filled in sequence, from the first element to the last element 
    - When the last element is filled, the index must reset before faulting the controller 
    - New variables will overwrite the old variables, starting again at the first element 
- Only one value can be stored in the Array
    - No "**double jumping**" of numbers is allowed
- Any values moved to the Output Module must be presented in the BINARY style radix. 
- On stop/restart, the output tag must revert to all zeroes.
    - The index position must also restart at zero.

*Proper rung documentation is mandatory.
