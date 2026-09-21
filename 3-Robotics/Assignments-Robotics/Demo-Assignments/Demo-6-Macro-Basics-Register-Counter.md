# MACRO BASICS (REGISTER COUNTER)

- We can use **Macro** keys to execute code without running in an active program!
- What's the difference between:
    - **User Key - UK**
    - **Shift Key - SK**
- In the "**Group Mask**" field, what is the purpose of setting:
    - the number one (1)
    - an asterisk (*)


## TASK
- Create (1) Macro to **count up** and store value in **REGISTER R**[1:Counter]
- Create (1) Macro to **count down** and store value in **REGISTER R**[1:Counter]
- Create (1) Macro to move the robot to a **SAFE POSITION**
    - Bind count **up** macro to **TOOL 1**
    - Bind count **down** macro to **TOOL 2**
    - Bind **safe** position macro to **MOVE MENU**

## FOCUS
- **Binding programs** as Macros to TP soft keys

## BASIC PARAMETERS
- Set program **DETAILS** to "*" for logic instead of "1" for Motion Groups
- Properly assign the Macro programs to the TP soft keys
    - [MENU] > [SETUP] > [MACRO]
- Assign Macro routines to the appropriate [PROGRAM]
    - Assign "**UK 1**" to Tool 1
    - Assign “**UK 2**” to Tool 2
    - Assign “**SU 3**” to Move Menu

## v1.0 - HARD-CODED LOGIC
- R[1: Counter] = R[1: Counter] **+** 1
- R[1: Counter] = R[1: Counter] **–** 1
    - _The constant **cannot be changed** when the program is running._

## v2.0 - SOFT-CODED LOGIC
- R[1: Counter] = R[1: Counter] **+** **R[2: Control]**
- R[1: Counter] = R[1: Counter] **–** **R[2: Control]**
    - _R[2:Control] **can** be changed when the program is running._


## NOTE

_Use a single Remark instead of the full Section format for these simple logic instructions._

## VIDEO REFERENCE

- Macro-1
