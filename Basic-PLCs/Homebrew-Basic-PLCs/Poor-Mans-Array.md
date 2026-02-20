# POOR MAN'S ARRAY

- In emulation, we can MOV a DINT to the Output Array (DINT) with a single instruction
    - Each individual BOOL of the DINT will MOV to the output module array BOOLs all at once
- We **cannot** MOV the DINTs to the lab IO output modules all at once
    - _Each output BOOL is nested within in its own separate "Channel" Data Type_ 
- To get around this, we use 16 XIC-OTE pairs, creating a "Poor Man's Array" of BOOLs
- The XICs are addressed to individual BOOLs of a single DINT; each BOOL is controlling a corresponding OTE addressed to single nested output BOOL:

### Example:
```text
    Output_Tag.0          Local:2:O.Pt00.Data
|------[ XIC ]------------------( OTE )------------|
    Output_Tag.1          Local:2:O.Pt01.Data
|------[ XIC ]------------------( OTE )------------|
    Output_Tag.2          Local:2:O.Pt02.Data
|------[ XIC ]------------------( OTE )------------|
    Output_Tag.3          Local:2:O.Pt03.Data
|------[ XIC ]------------------( OTE )------------|
    Output_Tag.4          Local:2:O.Pt04.Data
|------[ XIC ]------------------( OTE )------------|

and so on...
```

- Execute from .0 to .15 to cover all 16 Outputs of the 5069-OB16 output module
- Ensure to include the ".Data" at the end of each output, otherwise the MOV will fail

## Why all 16 outputs, and not just the ones we are using?

- _Because future assignments (Indirect Addressing, Sequencers, BSL/BSR, etc.) need all the outputs paired correctly for the visual effect to work as intended_

### Video Example of Morse Code:

[![Watch on YouTube](https://img.youtube.com/vi/keQ53TRdm9I/0.jpg)](https://youtu.be/keQ53TRdm9I)
