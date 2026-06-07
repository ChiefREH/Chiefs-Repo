# PICK-AND-PLACE (2 BOX / 1 TABLE)

## TASK
In **WORLD MODE**, record the following Points:
- **READY** position
- **APPROACH** position **100mm above** GREEN pick table
- **PICKUP** at Green position
- **APPROACH** position **100mm above** RED drop table
- **DROP** at Red position
- **SAFE position** _(away from both table)_ when finished

_Remember, the gripper will not animate properly unless the Main Program is run in **CYCLE MODE**_

## WORLD-BUILDING PARAMETERS
Include FIXTURE and PARTS:
- TABLE21
- RED Box
- BLUE Box

For this exercise, set **RO[1-2] COMPLIMENTARY = TRUE**

## SECTION SPECIFIC

```
!SETUP
- UTOOL_NUM = 1
- OVERRIDE = 50%
- R[1: Counter] = 0
- R[2: Control] = 4

!MAIN
- RO[1] = ON
- RO[1] = OFF
- R[1] = R[1] + 1
- IF R[1] = R[2] … END section
- IF R[1] > R[2] … ERROR section

!ERRORS
- UALM[1] “Count Exceeded”

!END OF LINE
- MESSAGE “Pick Program Complete”
```

## LAB PARAMETERS
- Verify the **Active Tool** and properly configured TCP distance / Orientation (direct entry)
- Must include both properly configured **Gripper Macros**
    - Bind to **TOOL 1** & **TOOL 2**

## VIDEO REFERENCE

- Animation-2-Box-1-Table
