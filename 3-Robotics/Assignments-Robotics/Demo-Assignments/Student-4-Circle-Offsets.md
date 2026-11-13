# CIRCLE OFFSETS
STUDENT ASSIGNMENT

## PARAMETERS

- **Target Height:** Z axis +100mm
- **Applied Offset:** +10mm
- **Cylinder Diameter**: 100mm


## WARNING
   
- DO NOT let the ROBOT make contact with any fixture, robot or other work-cell component.
    - This applies to any **Stop/Start/Restart** operations.
    - Doing so is an automatic failure.  **No exceptions**.
        - _If it looks close, then it's too close!_


## NOTE

- Benchie does not have the option for PR[i,j] in the IF/SELECT instruction menu
- We need this for the Z-axis high limit logic
- There is a workaround:
    - R[5] = PR[5,3]
    - _This will move the Z axis value into Register 5 (or whatever register you choose)_
- Apply logic using the Register instead of the PR[i,j]
    - IF R[5] >= 100, JMP LBL [999]

## VIDEO REFERENCE
- Assignment-Circle-Offsets
