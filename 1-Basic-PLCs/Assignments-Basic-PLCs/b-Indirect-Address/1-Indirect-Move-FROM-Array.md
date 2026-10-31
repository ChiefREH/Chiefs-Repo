# EMULATE Indirect Move FROM an Array

Create a routine that will pull a number **FROM** an Array and move the data to an Output module

## STATIC NUMBERS
Store these numbers in the DINT[16] array:
- 1, 2, 4, 8, 16, 32, 64, 128, 256, 512, 1024, 2048, 4096, 8192, 16384, 32768

## TIMING
- TON .PRE = 1 second 
- CTU .PRE = 16 

## PARAMETERS
- Once running, the routine must run continuously.
- All Array elements must be moved in order, from the first element to the last element. 
- When the last element is moved, the index must reset before faulting the controller. 
- Any values moved to the Output Module must be presented in the **BINARY** style radix. 
- On stop/restart, the output tag must revert to all zeroes.
    - The index position must also restart at zero.

*Proper rung documentation is mandatory.
