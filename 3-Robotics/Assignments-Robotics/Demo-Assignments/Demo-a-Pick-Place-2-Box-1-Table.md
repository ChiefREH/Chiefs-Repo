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
Include FIXTURE:
- TABLE21 at default world position
- Table21 Parts tab
    - RED Box
        - Create Delay = 2s
        - Destroy Delay = disabled
        - Visible at Teach Time / Visible at Run Time
    - BLUE Box
        - Destroy Delay = 2s
        - Create Delay = disabled
        - 

>We'll change the Delay to 3 seconds for both Boxes later.

Include a Gripper EOAT:
- Apply both Boxes in the EOAT Parts tab

>RED box should appear in the open gripper.

## SIMULATION SPECIFIC

- Pickup_RED_Simulation
    - Pickup RED, From TABLE21, With GRIPPER
- Drop_BLUE_Simulation
    - Drop BLUE, From GRIPPER, On TABLE21
- Drop_RED_Simulation
    - Drop RED, From GRIPPER

>The drop_red_sim will clear the red box from the gripper when the blue box appears on the table.

## SECTION SPECIFIC

```
!SETUP
- UTOOL_NUM = 1
- OVERRIDE = 100%
- R[1: Counter] = 0
- R[2: Control] = 3

- CALL Drop_RED_Simulation

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
- CALL Drop_RED_Simulation
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
