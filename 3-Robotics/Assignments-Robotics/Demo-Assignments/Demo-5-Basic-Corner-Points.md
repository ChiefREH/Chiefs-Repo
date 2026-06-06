# BASIC CORNER POINTS

## TASK
- Add an End-of-Arm-Tool (**EOAT**) to the robot (Pointer)
- Record a **SAFE** position away from the work area
- Record a **READY** position to serve as your starting point
- Record 4 corner points of a Table using the **WORLD** COORDINATE system (not JOINT mode)

## ROBOGUIDE PARAMETERS
- Include a properly configured **EOAT**
- Set the tool to ACTIVE in the Setup menu
- Include a properly placed **FIXTURE**

## FOCUS
- Use **REGISTERS** and **IF/THEN** logic to control the number of loops
- Using the Toolbar shortcut keys for different VIEWS of the robot
- **SPLIT SCREEN** to view the number of loops stored in the **REGISTER**

## SECTION SPECIFIC
**!SETUP**
- UTOOL_NUM = 1 for our new pointer
- Don’t forget to SETIND for this tool
- OVERRIDE =25% to slow down the speed of the routine
- REGISTER R[1] = for storing the number of required loops
- Include Register NAMES to differentiate each R[ ]

**!MAIN**
- LBL/JMP LBL instructions to loop the program
- IF/THEN LOGIC
- R[1] = R[1] + 1 <<< what I call an “adder”
- IF R[1] = 3 … JMP LBL [999]  <<< hard-coded/direct coding

**!ERRORS**
- UALM[1] for faulted conditions.

**!END OF LINE**
- Move the robot to the SAFE position
- MESSAGE for completed condition.

## VIDEO REFERENCE

- Roboguide-4
