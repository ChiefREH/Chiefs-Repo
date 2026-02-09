# TWO TON FLASHER AND SELECTOR SWITCH

Complete the following tasks:

- Properly wire a SELECTOR SWITCH (SSW)
- Properly wire in (2) Time-On TIMERS (TON) & BASES 
    - Set both Timers to ~3 seconds

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
	    |	        TON 1 N.O.	               TON 2 Coil		  |
	    |--------------[   ]--------------------( COIL )----------|
```
