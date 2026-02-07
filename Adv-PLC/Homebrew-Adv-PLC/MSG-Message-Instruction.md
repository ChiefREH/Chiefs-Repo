# MSG Message instruction

- Create a simple routine to activate a remote PLC using Ethernet communications:
- Properly configured MSG instructions 
- Properly configured Controller scope tags versus Local scope tags 

In Studio 5000 > F1 Help > search for “Specify the Communication Details”
This will give the formatting of the Message pathway

## CIP DATA TABLE WRITE
- MSG pathway format for emulation: add the 2nd emu controller to your I/O backplane and select as Path
- MSG pathway format for lab: "2, IP address of target PLC, 1, 0"


## CIP GENERIC PARAMETERS FOR VFDs
Get Attribute Single

- INSTANCE
    - 1 Frequency
    - 3 Current
    - 4 Voltage

- CLASS 93
- ATTRIBUTE 9

## PARAMETERS
- New Controller Scope Tags
- Divide by 100
- Destination: new Tag of the REAL Data type

Communication > Browse > Select your VFD


