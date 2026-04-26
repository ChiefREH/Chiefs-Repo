# BSL / BSR ASSIGNMENT - "Knight Rider"

Create a Bit Shift routine using any of the following instructions:
- All necessary XIC, XIO and/or ONS 
- TON - TIMER instructions 
- CTU - COUNTER instructions 
- ONS - ONE-SHOT instructions 
- BSL - BIT SHIFT LEFT instructions 
- BSR - BIT SHIFT RIGHT instructions 
- MOV - MOVE instructions
- COP - COPY instructions
- RES - RESET instructions 
- CLR - CLEAR instructions
- COMPARISON instructions 
- Properly created ARRAY(s) 

## PROGRAMMING TIP: 
Think of it as 3 separate steps:
1. Use a BSL to shift four 1s all the way down
2. Use a BSR to shift 0s all the way up
3. Use another BSL to shift 0s back down
- Repeat 2 and 3


## NOTES:
- "The KITT" sweeping sensor must be **4 bits wide** 
- The bits must feed into the "screen" 1 bit at a time and not "pop" into existence 
- The routine will operate using SEAL-IN circuit logic. 
- In the lab, this will be aliased to a physical Push Button. 
- Once started, the routine must continually loop 

*Proper rung documentation is mandatory.
