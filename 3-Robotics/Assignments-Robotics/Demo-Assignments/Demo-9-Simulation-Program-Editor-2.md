# COMBINE ANIMATION AND ROBOT OUTPUT RO[ ]

## TASK
- Animate an **OPEN** gripper operation with the Simulation Editor
- Animate a **CLOSE**D gripper operation with the Simulation Editor

## STEPS
- Add Robot to the work-cell
- Add Gripper CAD for Open and Closed
- Sim Editor
    - Create Pickup and Drop routines
        - _Notice there are no options_
- Add Table21
- Spawn in a BLUE BOX
- Add BOX to Table and EOAT
    - _Do the Pickup/Drop routines update?_
- Create a Main Loop simulation program to CALL the animated routines

```text
LBL [100]
- RO[1] = OFF
- RO[2] = ON
- CALL Z_Grip_PICK
- WAIT 2 sec
- RO[2] = OFF
- RO[1] = ON
- CALL Z_Grip_DROP
- WAIT 2 sec
JMP LBL [100]
```

- Split Screen to view RO when program is running
- Run the program in **CYCLE MODE** to see the animations function properly

## MOTION
- Record J P[1] 100% FINE at **100mm** ABOVE the BOX (Open/Drop)
- Use the **MoveTo** feature to position the robot directly at the BOX
- Record J P[2] 100% FINE at the BOX (Close/Pickup)

## CREATE / DESTROY
- Enable/Disable each option and view the results
- Adjust the **Create Delay** to 6 seconds and view the results
    - _Disable the **Destroy** at default 9999_

## MODIFICATION
- Loop the entire simulation program 3 times
    - _Replace LBL/JMP LBL with FOR/ENDFOR_

## QUESTION
- Can you assign/bind the animated routines to a Macro key?
- Will the Macro keys work in Cycle Mode?
- Will the animated routines work in the lab?



## VIDEO REFERENCE

- Roboguide-Gripper-Setup
