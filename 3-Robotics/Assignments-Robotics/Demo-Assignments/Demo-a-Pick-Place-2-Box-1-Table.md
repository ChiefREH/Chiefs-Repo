# PICK-AND-PLACE (2 BOX / 1 TABLE)

## TASK
In **WORLD MODE**, record the following Points:
- **READY** position
- **APPROACH** position **100mm above** RED BOX
- **PICKUP** at RED corner
- **APPROACH** position **100mm above** BLUE BOX
- **DROP** at BLUE corner
- **SAFE position** _(away from table)_ when finished

_Remember, the gripper will not animate properly unless the Main Program is run in **CYCLE MODE**_

## WORLD-BUILDING PARAMETERS
Include FIXTURE and PARTS:
- TABLE21
- RED Box
- BLUE Box


## SECTION SPECIFIC

```
!SETUP
- OVERRIDE = 50%
- R[1: Counter] = 0
- R[2: Control] = 3

!MAIN
- READY position
- APPROACH position above PICKUP
- At PICKUP position
    - RO[1] = OFF
    - RO[2] = ON
    - CALL Pickup_RED_Simulation
    - WAIT 2s
- APPROACH position above PICKUP
- READY position
- APPROACH position above DROP
- At DROP position
    - RO[2] = OFF
    - RO[1] = ON
    - CALL Drop_BLUE_Simulation
    - WAIT 2s
- APPROACH position above DROP
- READY position

- Logic for loop counting:
    - R[1: Counter] = R[1: Counter] + 1
    - IF R[1: Counter] = R[2: Control] … END OF LINE
    - IF R[1: Counter] > R[2: Control] … ERRORS

!ERRORS
- UALM[1] “Count Exceeded”

!END OF LINE
- SAFE position
- MESSAGE “Pick Program Complete”
```

## LAB PARAMETERS
- Verify the **Active Tool** and properly configured TCP distance / Orientation (direct entry)
- Must include both properly configured **Gripper Macros**
    - Bind to **TOOL 1** & **TOOL 2**

## VIDEO REFERENCE

- Animation-2-Box-1-Table
