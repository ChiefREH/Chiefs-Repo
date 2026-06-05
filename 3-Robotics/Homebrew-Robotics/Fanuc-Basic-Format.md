# MY FANUC FORMAT

This is the way I structure my simulation programs. I'm not saying it's the only way, it's just my way. When you're out in the real world, the structure will vary based on customer/employer requirements.

## ROBOGUIDE PARAMETERS

Accept *most defaults, with these exceptions: 

- Project name with YOUR initials
- Process Selection: **HandlingPro**
- Software Version: default (9.4 or higher)
- No EOAT attached (we'll add this later)
- Robot Model: **H755 - LR Mate 200iD**

_*Some options will vary by software version._


## PROGRAM SECTIONS

**!SETUP**
- Contains data that will only be executed once during start
- Can be hard-coded or placed in Registers

**!MAIN [LBL 100]**
- Contains the primary loop (Label and Jump Label)
- Performs all checks, looking for conditions
- Performs all movements (Joint, Linear, Circular)
- Waits for external inputs (Digital I/O)

**!ERROR [LBL 900]**
- When a faulted condition exists, the loop ends here
- Contains the User Alarm to notify the operator

**!END OF LINE [LBL 999]**
- When the run is complete and all conditions are normal
- Contains a Message instruction to notify the Operator

_All programs will be formatted with these four Sections. Future programs of higher complexity may have additional Sections as needed._
