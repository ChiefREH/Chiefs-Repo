# MACRO BASICS (ROBOT OUTPUTS RO)

## WORLD-BUILDING COMPONENTS
- Table21
- two Blue Boxes
    - one for the table top
    - one for the closed gripper model
- **Open** Gripper CAD model as the EOAT
- **Closed** Gripper CAD model to the EOAT
    - Demonstrate how to manually open/close gripper
    - Demonstrate how the animation does not work in code

## TASK
- **Measuring Tool** to determine size of the Blue Box for CLOSED gripper model
- Create 1 macro program to turn RO[1] OFF and RO[2] ON (Gripper Open)
- Create 1 macro program to turn RO[2] OFF and RO[1] ON (Gripper Closed
    - Bind the Open macro program to **TOOL 1**
    - Bind the Closed macro program to **TOOL 2**

## FOCUS
- Binding programs as Macros to TP soft keys
- I/O screen > [TYPE] > **Robot** for viewing the outputs

## BASIC PARAMETERS
- Set program **DETAILS** to * for logic instead of 1 for Motion Groups
- Properly assign the Macro programs to the TP soft keys
    - [MENU] > [SETUP] > [MACRO]
- Assign Macro routines to the appropriate [PROGRAM]
    - Assign "UK 1" to **Tool 1**
    - Assign “UK 2” to **Tool 2**
- I/O Screen to view RO[1] status change

## LOGIC

**OPEN MACRO**
- RO[1] = OFF <<< _must be off FIRST_
- RO[2] = ON

**CLOSED MACRO**
- RO[2] = OFF <<< _must be off FIRST_
- RO[1] = ON

_Why must the output be turned off before turning the next one on?_


## NOTES
- _Can we eliminate the need for this code by using **Complimentary Pairs**?_
- _Use a single Remark instead of the full Section format for these simple logic instructions._

## VIDEO REFERENCE

- Macro-2
