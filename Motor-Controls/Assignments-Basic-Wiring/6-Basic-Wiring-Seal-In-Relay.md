# RELAY AND SEAL-IN CIRCUIT

Complete the following tasks:
- Properly wire (2) sets of TERMINAL BLOCKS to the TRANSFORMER secondary (X1/F1 - X2) 
- X1/F1 will act as the POSITIVE polarity (supply line)
    - X2 will act as the NEGATIVE polarity (return line) 
- Properly wire (1) N.O. and (1) N.C. PUSH-BUTTON from the (+) TERMINAL BLOCK 
- Properly wire in (1) ICE-CUBE RELAY & BASE 
- Properly wire (2) LIGHTS to the RELAY contacts 
    - Properly wire the returns to X2 via the (-) TERMINAL BLOCK 
- Properly wire the components as a SEAL-IN CIRCUIT 
- Properly install the FUSES into the MAIN POWER DISCONNECT box 

*Troubleshoot as needed

NOTE:
- X1-F1 is made via the FUSE
- See Sketch #3 for details.

UPGRADE:
- _What happens if we replace the AB ice cube relay with an AB TON timer relay?_


## SIMPLE LADDER DIAGRAM

```text
F1     TB+	      NCPB          NOPB	      RELAY 1	         TB-	      X2
|-----[|||]------[ / ]---------[    ]---------( COIL )----------[|||]-----------|
	    |                |				  |				          |
        |                |  RELAY 1 NC#1  |                       |
        |                |-----[    ]-----|                       |
        |                                                         |
        |                                                         |
        |                                                         |
	    |	        RELAY 1 NC#2	             Red Light		  |
	    |--------------[ / ]-----------------------( R )----------|
	    |							                           	  |
	    |	        RELAY 1 NO#2	            Green Light		  |
	    |--------------[   ]-----------------------( G )----------|
```
