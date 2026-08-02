# POSITION REGISTERS (POINTER)

Create a program that uses all **PR[ ]** instead of **P[ ]**

## TASK
- Record **POSITION REGISTERS** PR[ ] for use in a routine
    - _Can go to a PR[ ] without running the program?_
    - _Changes made to the PR effects any Program using the PR!_

## FOCUS
- Record the **SAFE** position for PR[1] away from the FIXTURE
    - _Notice the R / * at the end of the entry?_
- Record a **READY** position for PR[2]
- Record a **APPROACH** position PR[3] **100mm above** the first corner
- Record all 4 corners as **POSITION REGISTERS** PR[ ]

## DATA PARAMETERS
- Use **REGISTERS** for soft-coding/indirect addressing
    - _Similar to indirect addressing in PLCs_

## SECTION SPECIFIC

```
!SETUP
- UTOOL_NUM = 1
- OVERRIDE = 25%
- R[1: Counter] = 0
- R[2: Control] = 3

!MAIN
LBL
- R[1: Counter] = R[1: Counter] + 1
- IF R[1: Counter] = R[2: Control] … JMP LBL [999]
- IF R[1: Counter] > R[2: Control] … JMP LBL [900]
JMP LBL
 
!ERRORS
- UALM[1] “Count Exceeded”

!END OF LINE
- Move to the SAFE position
- MESSAGE “Count Complete”
```

## VIDEO REFERENCE

- Roboguide-5
- Roboguide-6
