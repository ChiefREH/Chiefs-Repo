# Convert an Emulated Program to Lab Hardware
- Convert a Traffic routine with "Seal-In Circuit" control
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


--|   |--  N.O. Contact
--| / |--  N.C. Contact
--(   )--  COIL
```

## Question
- Does programming this wiring diagram yield the desired result?
- If not, what needs to change?
- Explain why the changes might be needed?
