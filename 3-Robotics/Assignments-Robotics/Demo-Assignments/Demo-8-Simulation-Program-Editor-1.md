# SIMULATION PROGRAM EDITOR

- Familiarize yourself with the **Simulation program Editor**
- Use **!** to include all necessary SECTIONS and REMARKS

## FOCUS
- Determine the **pros** (animation) and **cons** (limitations) of using the Sim Editor
    - Only runs in CYCLE MODE?
    - Can we run from the TP??

## MOTION TASKS
- Record a basic motion program:
    - P[1] READY position
    - P[2] APPROACH position 100mm above the table corner
    - P[3] to P[7] corner points:

```text
!SETUP
- J P[1] 100% FINE
- J P[2] 100% FINE

!MAIN LOOP
- LBL [100]
    - J P[3] 100% FINE
    - J P[4] 100% FINE
    - J P[5] 100% FINE
    - J P[6] 100% FINE
    - J P[7] 100% FINE
- JMP LBL [100]
```
- Cannot create a "dummy point" in the simulation editor
    - _Right-click, copy P[3], paste as P[7]_
 

## MOTION MODIFICATIONS

**!SETUP**
- Review the **WAIT** instruction
    - Include a WAIT DI[1]=ON
    - _Won’t work unless the input is set to SIM_

**!MAIN**
- Change all J P[ ] 100% FINE to **LINEAR P[ ] 250mm/sec FINE**
    - _Review the difference between Joint and Linear?_
- Replace LBL/JMP LBL with FOR/ENDFOR
    - FOR R[1] = 1 to 3
    - ENDFOR



## VIDEO REFERENCE
- Sim-Editor-1 
- Sim-Editor-2
