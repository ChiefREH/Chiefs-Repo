# EMULATE Indirect Move TO an Array with RTO as RNG

Create a routine that will move a variable number into a DINT[10] Array sequentially


## TIMING
- TON .PRE = 1 second 
- RTO .PRE = 32,767 seconds 
- CTU .PRE = 10 

## PARAMETERS
- Once running, the routine must run continuously
- All Array elements must be filled in sequence, from the **first** element to the **last** element
- Only one value can be stored in the Array
    - No "**double jumping**" of numbers is allowed
- When the last element is filled, the index must reset **before** faulting the controller
- New variables will overwrite the old variables, starting again at the first element
- On stop/restart, the output tag must revert to all zeroes
    - The index position must also restart at zero

*Proper rung documentation is mandatory.
