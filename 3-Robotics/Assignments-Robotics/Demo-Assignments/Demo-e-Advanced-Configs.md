# ADVANCED PROGRAMMING CONFIGURATION

Create a 4-corner tracing Program using Table21 and a blue Box 100/100/30mm

RUN IN CYCLE MODE

## TASK:
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

## Control the Program with a Time Out:
- WAIT (DI[1]) TIMEOUT, LBL [950]
- TIMEOUT located in MENU > next > SYSTEM > VARIABLES > $WAITTMOUT
- Measured in hundredths of a second.
- Default is 3000 = 30 seconds

## CLONE a full Robot model
- Right-click C:1 Robot Controller > Add Robot > Add Robot Clone
- Accept default location parameters.
- Properly configured DI and DO interface

## Cell > I/O Interconnections > Work-cell I/O
- Controller 2 DO[1] > Controller 1 DI[1]
- At the end: Controller 1 DO[1] > Controller 2 DI[1]

## Control a Robot remotely with Digital Inputs:
- ROBOT 1: WAIT DI=ON
- ROBOT 2: Doesn’t need a Program, just toggle the I/O
- Split Screen bot Inputs and Outputs

## SECTION SPECIFIC

!SETUP:
UTOOL_NUM=1  (SETIND for UTOOL_NUM and USERFRAME_NUM)
UFRAME=1
OVERRIDE=50%

!READY POSITION
P[1] Ready position
WAIT (DI[1]) TIMEOUT, LBL [950]
Before Cloning: WAIT DI[1]=ON

!MAIN:
LBL [100]
All 4 corner points. Return to Ready position.
JMP LBL [999]

!ERRORS:
LBL [900]
Nothing.
LBL [950]
UALM 2 (“Wait Time Elapsed”)

!END OF LINE:
LBL [999]
R[7:Month]=($SYS_TIME.$MONTH)
R[8:Day]=($SYS_TIME.$DAY)
R[9:Hour]=($SYS_TIME.$HOUR)
R[10:Minute]=($SYS_TIME.$MINUTE)
Robot 1 >>> DO[1]=ON signal to Robot 2

## VIDEO REFERENCE
- Adv-Configs-1
- Adv-Configs-2
