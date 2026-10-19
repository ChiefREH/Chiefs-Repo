# CREATE USERFRAMES

_Cannot move tables around Big Yella and Benchie, so I limit this exercise to Roboguide._

## TASK
Teach a UFRAME_NUM origin for a fixture (**Table-With-Legs**) in the world
1. **SETIND** for your new UFRAME number
2. Set one BOX on the Table and record all the top corner Points
3. **Move** the Fixture to a different location in the World
4. When directed, **touch up** the UserFrame origin coordinates using the **Three-Point Method**
5. **TOUCH UP** P[1] before running the program
    - _So the robot doesn’t fault on a Servo Limit alarm_
6. Verify the box tracing Program works properly in the new location


## ROBOGUIDE PARAMETERS
- Part: Blue "Box"
- Fixture Model: **"Table-With-Legs”**


## TEACH PENDANT / MENU PARAMETERS
- Coordinates: **WORLD**
- Active Frames: Tool Frame 1 & User Frame 1
    - **UFrame** must be taught first (**Three-Point Method**)

## SECTION SPECIFIC

```
!SETUP
- UTOOL_NUM = 1 (SETIND)
- UFRAME_NUM = 1 (SETIND)
- OVERRIDE = 25%
- PAYLOAD[1]
    - MENU > next > SYSTEM > Motion

!MAIN
- Record APPROACH point 100mm above the box's starting point
- Record Corner Points
    - J P[ ] 100% FINE
- Change to Linear for more precise travel

!ERRORS
- Remark & Label only. No code needed.

!END OF LINE
- Remark & Label only. No code needed.
```

## VIDEO REFERENCE
- Teach-UserFrame
