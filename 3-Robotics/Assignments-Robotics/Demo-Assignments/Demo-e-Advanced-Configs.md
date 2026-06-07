# ADVANCED PROGRAMMING CONFIGURATION

Create a 4-corner tracing Program using Table21 and a blue Box

Remember to run both in **CYCLE MODE**

## TASK
Install Optional Package "Internet Conn/Custo (R558)"
- Right-click LR MATE 200iD > Properties > Serialize
- **DO NOT** use SERIALIZE WIZARD. It will add a NEW robot!

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

## Clone a full Robot model
Right-click C:1 Robot Controller > Add Robot > Add Robot Clone
- Accept default location parameters.
- Properly configured DI and DO interface

## Cell > I/O Interconnections > Work-cell I/O
- Controller 2 DO[1] > Controller 1 DI[1]
- Controller 1 DO[1] > Controller 2 DI[1]

## Control a Robot remotely with Digital Inputs
- ROBOT 1: WAIT **DI[1] = ON**
- ROBOT 2: Doesn’t need a Program, just toggle **DO[1]**
    - Split Screen both Inputs and Outputs

## SECTION SPECIFIC
```
!SETUP
- UTOOL_NUM = 1
- UFRAME = 1
- OVERRIDE = 50%
- DO[1] = OFF

!READY POSITION
LBL [50]
- Move to P[1] READY position
- WAIT (DI[1]) TIMEOUT, LBL [950]

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

NOTE
- Adjust the default TIMEOUT to 1000 (10 seconds)

## VIDEO REFERENCE
- Adv-Configs-1
- Adv-Configs-2
