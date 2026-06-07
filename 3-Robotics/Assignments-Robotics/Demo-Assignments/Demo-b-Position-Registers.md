# POSITION REGISTERS (POINTER)

## TASK
- Record POSITION REGISTERS PR[ ] for use in a routine
- Can go to a PR[ ] without running the program!
- Changes made to the PR effects any Program using the PR!

## FOCUS
- Record the SAFE position for PR[1] safely away from the FIXTURE
- Notice the R / * at the end of the entry?
- Record a READY position for PR[2]
- Record a PERCH position PR[3] 100mm above the first corner
- Record all 4 corners as POSITION REGISTERS PR[ ]
- Create a program that uses all these PR[ ] instead of P[ ]

## DATA PARAMETERS
- REGISTER R[2: Control] = 3 for comparing/modifying the requested loops
- Soft-coding/indirect addressing
- What happens if you change the CONTROL to a value lower than completed loops?

## SECTION SPECIFIC

```
!SETUP
- UTOOL_NUM = 1
- OVERRIDE=25%
- REGISTER R[1] = 0

!MAIN
LBL
- R[1] = R[1] + 1
- IF R[1: Counter] = R[2: Control] … JMP LBL [999]
- IF R[1: Counter] > R[2: Control] … JMP LBL [900]
JMP LBL
 
!ERRORS
- UALM[1] “Count Exceeded”

!END OF LINE
- Move the robot to the SAFE position
- MESSAGE “Count Complete”
```

## VIDEO REFERENCE

- Roboguide-5
- Roboguide-6
