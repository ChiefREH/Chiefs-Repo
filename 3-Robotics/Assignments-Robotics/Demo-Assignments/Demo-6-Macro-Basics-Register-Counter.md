# MACRO BASICS (REGISTER COUNTER)

- Can use **Macro** keys to execute code without running in an active program!
    - Difference between **UK** and **SK** ??

## TASK
- Create (1) program to **count up** and store value in **REGISTER R**[1]
- Create (1) program to **count down** and store value in **REGISTER R**[1]
- Create (1) program to move the robot to a **SAFE POSITION**
    - Bind count up program to **TOOL 1**
    - Bind count down program to **TOOL 2**
    - Bind safe position program to **MOVE MENU**

## FOCUS
- **Binding programs** as Macros to TP soft keys

## BASIC PARAMETERS
- Set program **DETAILS** to * for logic instead of 1 for Motion Groups
- Properly assign the Macro programs to the TP soft keys
    - [MENU] > [SETUP] > [MACRO]
- Assign Macro routines to the appropriate [PROGRAM]
    - Assign "**UK 1**" to Tool 1
    - Assign “**UK 2**” to Tool 2
    - Assign “**SU 3**” to Move Menu

## HARD-CODED LOGIC
- R[1: Counter] = R[1: Counter] + 1
- R[1: Counter] = R[1: Counter] – 1
    - The constant **cannot be changed** when the program is running.

## SOFT-CODED LOGIC
- R[1: Counter] = R[1: Counter] + R[2: Control]
- R[1: Counter] = R[1: Counter] – R[2: Control]
    - _R[2] **can** be changed on the fly when the program is running._


_Use a single Remark instead of the full Section format for these simple logic instructions._

## VIDEO REFERENCE

- Macro-1
