# ADVANCED PROGRAMMING CONFIGURATION II

>Use the previous program for this demo.


## Clone a full Robot model
Right-click C:1 Robot Controller > Add Robot > Add Robot Clone
- Accept default location parameters.
- Properly configured DI and DO interface

## Cell > I/O Interconnections > Work-cell I/O
- Controller 2 DO[1] > Controller 1 DI[1]
- Controller 1 DO[1] > Controller 2 DI[1]

## Control a Robot remotely with Digital Inputs

MANUAL CONTROL
- ROBOT 1: WAIT **DI[1] = ON**
- ROBOT 2: Doesn’t need a Program, just toggle **DO[1]**
    - Split Screen both Inputs and Outputs

AUTOMATED ROUTINE
- See Codes below

## ROBOT 1 ROUTINE
```
!SETUP
- OVERRIDE = 50%
- DO[1] = OFF
- R[1] = 0

!READY POSITION
LBL [50]
- P[1] READY position
- P[2] APPROACH position
- WAIT DI[1] = ON

!MAIN
LBL [100]
- P[3], P[4], P[5], P[6], P[3]
- R[1] = R[1] + 1
- IF R[1] >= 3, JMP LBL [999]
- JMP LBL [100]

!ERRORS
LBL [900]
- None for this exercise.

LBL [950]
- UALM 2 (“Wait Time Elapsed”)

!END OF LINE
LBL [999]
- Move to a SAFE position
- R[7:Month] = ($SYS_TIME.$MONTH)
- R[8:Day] = ($SYS_TIME.$DAY)
- R[9:Hour] = ($SYS_TIME.$HOUR)
- R[10:Minute] = ($SYS_TIME.$MINUTE)

- DO[1] = ON to signal the other robot
- WAIT 1 sec
- DO[1] = OFF to stop signaling
- WAIT 1 sec
- JMP LBL [50]
```

## ROBOT 2 ROUTINE
```
!SETUP
- UTOOL_NUM = 1
- UFRAME = 1
- OVERRIDE = 50%
- DO[1] = OFF

!READY POSITION
LBL [50]
- Move to P[1] READY position
- WAIT DI[1] = ON

!MAIN
LBL [100]
- All 4 corner points. Return to READY position.
- JMP LBL [999]

!ERRORS
LBL [900]
- None for this exercise.

LBL [950]
- UALM 2 (“Wait Time Elapsed”)

!END OF LINE
LBL [999]
- Move to a SAFE position
- R[7:Month] = ($SYS_TIME.$MONTH)
- R[8:Day] = ($SYS_TIME.$DAY)
- R[9:Hour] = ($SYS_TIME.$HOUR)
- R[10:Minute] = ($SYS_TIME.$MINUTE)
- DO[1] = ON to signal the other robot
- WAIT 3 sec
- DO[1] = OFF to stop signaling
```

---

NOTE
- Adjust the default TIMEOUT to 1000 (10 seconds)

## VIDEO REFERENCE
- Adv-Configs-1
- Adv-Configs-2
