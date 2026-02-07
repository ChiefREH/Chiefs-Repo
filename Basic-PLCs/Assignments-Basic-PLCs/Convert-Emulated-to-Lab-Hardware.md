# Convert an Emulated Program to Lab Hardware
- Convert a 4-Way Traffic routine with "Seal-In Circuit" control
    - Properly tag and alias XIO and XIC instructions to INPUT module push-buttons
    - Properly tag and alias the OTEs to the OUTPUT module lights
    - Add BRANCHES for multiple ALIASED OTE groups



## LADDER DIAGRAM OF A SIMPLE SEAL-IN CIRCUIT:

```text
L1        STOP             START              RUN          L2
|---------| / |------------|   |-------------(   )----------|
                    |                  | 
                    |       RUN        |
                    |------|   |-------|


--|   |--  XIC / N.O. Contact
--| / |--  XIO / N.C. Contact
--(   )--  OTE / COIL
```


