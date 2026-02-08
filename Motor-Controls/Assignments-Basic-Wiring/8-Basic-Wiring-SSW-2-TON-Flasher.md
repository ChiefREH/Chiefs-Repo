# TWO TON FLASHER AND SELECTOR SWITCH

Complete the following tasks:
- Properly wire (2) sets of TERMINAL BLOCKS to the TRANSFORMER secondary (X1/F1 - X2) 
- X1/F1 will act as the POSITIVE polarity (supply line)
    - X2 will act as the NEGATIVE polarity (return line) 
- Properly wire a SELECTOR SWITCH (SSW) from the (+) TERMINAL BLOCK 
- Properly wire in (2) Time-On TIMERS (TON) & BASES 
    - Set both Timers to ~3 seconds 
- Properly wire (2) LIGHTS to the RELAY 
    - Properly wire the returns to X2 via the (-) TERMINAL BLOCK 
- Properly install the FUSES into the MAIN POWER DISCONNECT box 

*Troubleshoot as needed

NOTE:
- X1-F1 is made via the FUSE
- See Sketch #4 for details.


## SIMPLE LADDER DIAGRAM

```text
F1     TB+	    SSW	        TON 2 N.C.     TON 1 Coil		     TB-	 X2
|-----[|||]----[    ]---------[ / ]---------( COIL )------------[|||]-----|
	    |								                          |
	    |	        TON 1 N.C.	                 Red Light		  |
	    |--------------[ / ]-----------------------( R )----------|
	    |							                           	  |
	    |	        TON 1 N.O.	                Green Light		  |
	    |--------------[   ]-----------------------( G )----------|
        |							                           	  |
	    |	        TON 1 N.O.	               TON 1 Coil		  |
	    |--------------[   ]--------------------( COIL )----------|
```
