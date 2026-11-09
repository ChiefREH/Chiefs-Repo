# CIRCLES FOR WELDING APPLICATION (POINTER)

![Circle Concept](Demo-Images/Circle-Concept.png)

## TASK
- Trace a circle around the end of a cylinder.
 
## WORLD-BUILDING PARAMETERS
- Fixture Model: "Table21”
- Part: Blue CYLINDER

## TEACH PENDANT / MENU PARAMETERS
- Coordinates: **WORLD**
- Active Frames: Tool Frame 1 & UserFrame 1
- **UFRAME 0** is "No Frame"

_If UTOOL or UFRAME causes and error ("Big Yella"), omit them both and move on!_

## SECTION SPECIFIC
```
!SETUP
- UTOOL_NUM = 1
- USERFRAME = 1
- OVERRIDE = 25%
- R[1: Count] = 0

- P[1] READY POSITION
- P[2] APPROACH POSITION 100mm above

!MAIN
LBL
- Record all needed CIRCULAR points
    - C P[] 250mm/sec FINE

- IF/SELECT logic for 3 loops
JMP LBL

!ERRORS
- Remark & Label only. No UALM needed.
 
!END OF LINE
LBL [999]
- P[7] SAFE POSITION
```

**QUESTIONS**
- _Notice the pause between each arc?_
- _How can we eliminate the pause?_
    - _Change 1st point on Circle to LINEAR 250mm/sec **CNT100** ?_


## LAB PARAMETERS
- Properly configured **Gripper MACROS** (Tool 1 & Tool 2) are required to hold the Pointer
- Verify the UTOOL_NUM is properly entered for your Robot


## VIDEO REFERENCE
- Circles
