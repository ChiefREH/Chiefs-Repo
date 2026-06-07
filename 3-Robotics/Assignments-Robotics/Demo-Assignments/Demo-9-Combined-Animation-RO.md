# COMBINE ANIMATION AND ROBOT OUTPUT RO[ ]

## TASK
- Add an open and closed gripper CAD model to the EOAT
- Animate an OPEN gripper operation with the Simulation Editor
- Animate a CLOSED gripper operation with the Simulation Editor

## FOCUS
- Properly assigning the BOX to the EOAT and FIXTURE
- Demonstrate **Create Delay** (6 sec) and **Destroy Delay** (6 sec)
- Use **CALL** instructions to make use of SIM EDITOR programs
- Use **WAIT** instructions to slow the program down for viewing
- Split Screen to view RO when program is running
- Run the program in **CYCLE MODE** to see the animations function properly

## SECTION SPECIFIC
**!SETUP**
- Remark & Label only. No code needed.

**!MAIN**

```text
LBL [100]
RO[1] = OFF
RO[2] = ON
CALL Z_Grip_PICK
WAIT 6 sec
RO[2] = OFF
RO[1] = ON
CALL Z_Grip_DROP
WAIT 6 sec
JMP LBL [100]
```

NOTE
- The **CALL** instruction is needed for the animation/simulation
- A 6 second **WAIT** is best for viewing the Create/Destroy delay

**!ERRORS**
- Remark & Label only. No code needed.

**!END OF LINE**
- Remark & Label only. No code needed.


## LAB PARAMETERS
None. Simulation Editor only.

## VIDEO REFERENCE

- Roboguide-Gripper-Setup
