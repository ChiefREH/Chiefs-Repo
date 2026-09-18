# CORNER POINTS WITH LOGIC

## TASK
- Add an End-of-Arm-Tool (**EOAT**) to the robot (Pointer)
- Record a **READY** position to serve as your starting point
- Record an **APPROACH** position that is **100mm** above the first Table corner
- Record 4 corner points of a Table using the **WORLD** COORDINATE system
    - _Not JOINT mode_
- Record a **SAFE** position away from the work area

## ROBOGUIDE PARAMETERS
- Include a properly configured **EOAT**
- Set the tool to **ACTIVE** in the Setup menu
- Include a properly placed **FIXTURE**

## FOCUS
- Use **DATA REGISTERS** and **IF/SELECT** logic to control the number of loops
- Using the Toolbar shortcut keys for different **VIEWS** of the robot
- **SPLIT SCREEN** to view the number of loops stored in the **REGISTER**

## SECTION SPECIFIC

**!SETUP**
- **UTOOL_NUM** = 1 for our new pointer
    - _Don’t forget to **SETIND** for this tool_
- **OVERRIDE = 50%** to slow down the speed of the routine
- **REGISTER R[1:Counter]** = 0
    - _This resets the Register to 0 on start_
    - _Include Register NAMES to differentiate each R[ ]_
- Record the **READY** position here at **P**[1]
- Record the **APPROACH** position here at **P**[2]

**!MAIN**
- **LBL** [100]
- Record 4 table corner positions:
    - **P**[3], **P**[4], **P**[5], **P**[6], **P**[3]
- Data Register math function:
    - **R**[1:Counter] = **R**[1:Counter] **+ 1** 
- **IF/SELECT** logic:
    - IF **R**[1:Counter] **=** 3, **JMP LBL** [999]
    - IF **R**[1:Counter] **>** 3, **JMP LBL** [900]
- **JMP LBL** [100]

**!ERRORS**
- **LBL** [900]
- **UALM**[1] for faulted condition alarm.


**!END OF LINE**
- **LBL** [999]
- Record the **SAFE** position here at **P**[7]
- **MESSAGE** for completed condition.


## VIDEO REFERENCE

- Roboguide-4
