# PICK-AND-PLACE (2 BOX / 1 TABLE)

## TASK
In WORLD MODE, record the following Points:
READY position
PERCH position 100mm above GREEN pick table
PICKUP at Green position (slow the speed to smooth the animation)
PERCH position 100mm above RED drop table
DROP at Red position (slow the speed to smooth the animation)
SAFE position (away from both tables)
The gripper will not animate properly unless the Main Program is run in CYCLE MODE

## FOCUS
Include FIXTURE and PARTS
TABLE21: 0.5/0.5/1.0 scale @ 400/0/300
RED Box: 1kg/30/30/30mm @ -120/-150/+30
BLUE Box: 1kg/30/30/30mm @ +120/+150/+30
RO[1-2] COMPLIMENTARY = TRUE

## SECTION SPECIFIC
!SETUP
UTOOL_NUM = 1
OVERRIDE = 50%
R[1: Counter] = 0
R[2: Control] = 4

!MAIN
RO[1] = ON
RO[1] = OFF
LOGIC
R[1] = R[1] + 1
IF R[1] = R[2] … END section
IF R[1] > R[2] … ERROR section

!ERRORS
UALM[1] “Count Exceeded”

!END OF LINE
MESSAGE “Pick Program Complete”

## LAB PARAMETERS
Verify the Active Tool and properly configured TCP distance / Orientation (direct entry)
Must include both properly configured Gripper Macros (bind to TOOL 1 & TOOL 2)

## VIDEO REFERENCE

- Animation-2-Box-1-Table
