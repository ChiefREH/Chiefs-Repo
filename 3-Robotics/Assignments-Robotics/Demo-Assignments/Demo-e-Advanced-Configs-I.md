# ADVANCED PROGRAMMING CONFIGURATION I

Create a 4-corner tracing Program using Table21 and a blue Box

Remember to run both in **CYCLE MODE**

## TASK
Install Optional Package "Internet Conn/Custo (R558)"
- If you forget to add the package during project creation:
    - Right-click LR MATE 200iD > Properties > Serialize

Use Registers to store **$SYS_TIME** variables (option R558) when the routine is done:
```
$SYS_TIME.$MONTH
$SYS_TIME.$DAY
$SYS_TIME.$HOUR
$SYS_TIME.$MINUTE
```
 
 NOTE
 - Mixed Logic Register adds a “$” to the beginning of the “Parameter”
 - SHIFT+DISP for Split Screen with Data Registers

## Control the Program with a Time Out
- **WAIT (DI[1]) TIMEOUT, LBL [950]**
    - **TIMEOUT** located in MENU > next > SYSTEM > VARIABLES > **$WAITTMOUT**
    - Measured in hundredths of a second.
    - Default is 3000 = 30 seconds

## ROBOT 1 ROUTINE
```
!SETUP
- UTOOL_NUM = 1
- UFRAME = 1
- OVERRIDE = 25%
- DO[1] = OFF

!READY POSITION
LBL [50]
- Move to P[1] READY position
- WAIT (DI[1]) TIMEOUT, LBL [950]

!MAIN
LBL [100]
- Run all 4 corner points ONE TIME ONLY
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
```

NOTE
- Adjust the default TIMEOUT to 1000 (10 seconds)

## VIDEO REFERENCE
- Adv-Configs-1
- Adv-Configs-2
