# BASIC PLC FINAL PROGRAM

- Create a Morse Code ticker using the **BSL instruction** as the primary operator
- "Stream" the phrase **"Hello World"** across the output module LEDs

## CODE:

Use the following instructions as needed:
- All necessary XIC, XIO and/or ONS 
- TON - TIMER instructions 
- CTU - COUNTER instructions 
- ONS - ONE-SHOT instructions 
- BSL - BIT SHIFT LEFT instructions 
- MOV - MOVE instructions
- COP - COPY instructions
- RES - RESET instructions 
- CLR - CLEAR instructions
- COMPARISON instructions
- MATH instructions
- Properly created ARRAY(s)
- Direct and/or Indirect Addressing (Index)

## SPECIFICATIONS:

- Bits must "stream" into the IO LEDs 1 letter at a time.
- Bits must "stream" into the IO LEDs, not just "pop" into existence!
- No SQO instructions are permitted.

## PARAMETERS:

- The routine will operate using SEAL-IN circuit logic.
    - In the lab, this will be aliased to a physical Push Button.
- Once started, the routine must continually loop until stop is pressed.
- Requires properly configured I/O modules for visual feedback (emulated and lab).

*Proper rung documentation is mandatory.