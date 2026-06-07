# POSITION REGISTER OFFSETS (PALLETIZING)

Trace a rectangle pattern with an increasing Z coordinate of +5mm

## TASK
Properly configure a **PR [ i , j ]** Offset:
- i = which **PR[ ]** to look at in the **DATA** list
- j = which **coordinate** inside the **PR[ ]** to look at:
    - X = 1
    - Y = 2
    - Z = 3 < _we will modify this coordinate_
    - W = 4
    - P = 5
    - R = 6

## WORLD-BUILDING PARAMETERS
- Parts: Generic BLUE_Box
- Fixture Model: Table21


## TEACH PENDANT / MENU PARAMETERS
- Coordinates: **WORLD**
- Active Frames: Tool Frame 1 & User Frame 1
- Zero out all PR[ ] Coords:
    - PR[5: Z OFFSET] > [POSITION] > manually enter "0" for XYZ WPR coordinates > [DONE]
        - _This is a new twist on PR[ ]_


## SECTION SPECIFIC

```
!SETUP
- UTOOL_NUM = 1
- OVERRIDE = 50%
- PR[5,3:Z OFFSET] = 0  						

!MAIN
LBL
- Record all needed MOTION points
    - L P[ ] 250mm/sec FINE for the 4 box corners
- All box corners are recorded, add Offset, PR[5] to each      
    - PR[5,3:Z OFFSET] = PR[5,3:Z OFFSET] + 5 
- IF PR[5,3:Z OFFSET] => 300 JMP LBL 999
    - This is a "safety fence"
JMP LBL

!ERRORS
- None for this exercise

!END OF LINE
- Go to a SAFE position
    - This position must be away from the offset "stack"
    - Does not require a PR, CALL or a SAFE MACRO
```

**QUESTIONS**
- _Can we replace the hard-coded constant "5" with a Register?_
- _Why would we want to replace the constant?_
- _What happens if the Register stores a negative number?_
- _Should we rely on code alone for robot motion safety?_

## LAB PARAMETERS
- Properly configured **Gripper MACROS** (Tool 1 & Tool 2) are required to hold the Pointer
- Verify the **UTOOL** data is properly entered for your robot
- If you get an **"Invalid Frame Error"** in the lab, set your user frame to UFRAME = 1

_If Toolframe 1 or Userframe 1 create problems, we will omit them and carry on!_

## WARNING
- DO NOT let the EOAT make contact with any part, fixture or work area.
- Doing so is an automatic failure. No exceptions.

## VIDEO REFERENCE

- PR-Offsets
