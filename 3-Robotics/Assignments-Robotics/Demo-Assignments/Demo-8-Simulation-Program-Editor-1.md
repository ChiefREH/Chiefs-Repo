# SIMULATION PROGRAM EDITOR

- Familiarize yourself with the **Simulation program Editor**
- Use **!** to include all necessary SECTIONS and REMARKS

## MOTION TASKS
- Record a basic program:
    - READY position
    - APPROACH position 100mm above the table corner
    - Four corner points

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

- Modify the points:
    - JOINT P[ ] 100% FINE to **LINEAR P[ ] 250mm/sec FINE**
        - _What's the difference between Joint and Linear?_

## FOCUS
- Familiarize with the **pros** (animation) and **cons** (limitations) of using the Sim Editor
    - Only runs in CYCLE MODE?
    - Can we run from the TP??

## SECTION SPECIFIC

**!SETUP**
- Review the **WAIT** instruction
    - Include a WAIT DI[1]=ON
    - _Won’t work unless the input is set to SIM_

**!MAIN**
- FOR LOOP LOGIC
    - FOR R[1] = 1 to 3
    - ENDFOR to loop the program x3
        - This can replace LBL/JMP LBL

**!ERRORS**
- Remark & Label only. No code needed.

**!END OF LINE**
- Remark & Label only. No code needed.


## VIDEO REFERENCE
- Sim-Editor-1 
- Sim-Editor-2
