# PROXIMITY SENSOR

Complete the following tasks:
- Properly wire (2) sets of TERMINAL BLOCKS to the TRANSFORMER secondary (X1/F1 - X2) 
- X1/F1 will act as the POSITIVE polarity (supply line)
    - X2 will act as the NEGATIVE polarity (return line) 
- Properly wire in a SENSOR or PHOTO EYE with N.C. and N.O. contacts 
- Properly wire (2) LIGHTS to the sensor's contacts 
    - Properly wire the returns to X2 via the (-) TERMINAL BLOCK 
- Properly install the FUSES into the MAIN POWER DISCONNECT box 

*Troubleshoot as needed

NOTE:
- X1-F1 is made via the FUSE
- See Sketch #17 for details.


## SIMPLE LADDER DIAGRAM

```text
F1     TB+	                 PROX SW	                  TB-	       X2
|-----[|||]----------------( SENSOR )--------------------[|||]-----------|
	    |								                   |
	    |	        SENSOR N.C.	          Red Light		   |
	    |--------------[ / ]----------------( R )----------|
	    |							                       |
	    |	        SENSOR N.O.	          Green Light	   |
	    |--------------[   ]-----------------( G )---------|
```
