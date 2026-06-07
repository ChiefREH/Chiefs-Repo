# POSITION REGISTER OFFSETS (PALLETIZING)

Trace a rectangle pattern with an increasing +Z height

## TASK
Properly configure a PR [ i , j ] Offset to add +5mm to the Z coordinate every loop
i = which PR to look at in the DATA list
j = which coordinate inside the PR to look at:
X = 1
Y = 2
Z = 3
W = 4
P = 5
R = 6

## ROBOGUIDE PARAMETERS
Parts: Generic BLUE_Box: SCALE XYZ 100 mm/100 mm/30 mm/1 kg
Fixture Model: Table21 (Scale: 0.5/0.5/0.5 // LOC: 400/0/300)
Part Offset > Generic BLUE_Box: Z +30 mm

## TEACH PENDANT / MENU PARAMETERS
Coordinates: WORLD
Active Frames: Tool Frame 1 & User Frame 1
PR[5: Z OFFSET] > [POSITION] > manually change XYZ WPR to all 0 > [DONE]
This is a new twist on PR[ ]

## SECTION SPECIFIC
!SETUP section includes:
UTOOL_NUM=1
OVERRIDE=50%			< Consider a faster speed so the routine takes less time
PR[5,3:Z OFFSET]=0  						< This is a new Register

!MAIN section [100]
Proper LBL/JMP LBL
Record all needed MOTION points
L P[ ] 250mm/sec FINE for the 4 box corners
All box corners are recorded, add Offset, PR[5] to each path      < This is a new instruction
PR[5,3:Z OFFSET]=PR[5,3:Z OFFSET]+5  			        < This is new logic
IF PR[5,3:Z OFFSET] => 300 JMP LBL 999 					< Safety Fence

!ERROR HANDLING section
None for this exercise

!END OF LINE section [999]
Go to a SAFE position
This position must be away from the stack
Does not require a PR, CALL or a SAFE MACRO

## LAB PARAMETERS
Properly configured Gripper MACROS (Tool 1 & Tool 2) are required to hold the Pointer
Verify the UTOOL data is properly entered for your robot
If you get an "Invalid Frame Error" in the lab, set your user frame to UFRAME = 1

## WARNING
DO NOT let the EOAT make contact with any part, fixture or work area.
Doing so is an automatic failure.

## VIDEO REFERENCE

- PR-Offsets

