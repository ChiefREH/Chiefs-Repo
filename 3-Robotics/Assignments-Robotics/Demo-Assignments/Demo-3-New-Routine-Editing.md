# NEW ROUTINE & EDITING (NO EOAT)

## TASK

- Record a minimum of 4 points using the **WORLD** coordinate system
- Can we reposition points already created?
    - Touchup from the TP??


## PROGRAM SECTIONS

A standard Routine will **always** contain four (4) Sections:

- **!SETUP:** Instructions that run once at start
- **!MAIN [100]:** Instructions that loop
- **!ERRORS [900]:** Alert the operator of faulty conditions
- **!END OF LINE [999]:** When all instructions are complete

_All programs will be formatted with these four Sections. Future programs of higher complexity may have additional Sections as needed._


## FOCUS

- Use **INST/EDCMD** to format Sections with **REMARKS**
- **SHIFT / RESET / FWD / BWD** to run a program
    - What happens when recording points with SHIFT toggled?
    - What happens when running BWD in the program?
- **HOLD** to stop the routine (or release dead-man switch)
- **STEP** mode for troubleshooting
    - Notice the @ symbol in the program?
- **FCTN > ABORT (ALL)** to kill a program running in the background
- Export your Routine as an .LS file


## SECTION SPECIFIC

### !SETUP
- **OVERRIDE** = 25% to slow down the speed of the routine

### !MAIN
- **LBL/JMP LBL** instructions to loop the routine

### !ERRORS
- Remark & Label only. No code needed

### !END OF LINE
- Remark & Label only. No code needed



## VIDEO REFERENCE

- Roboguide-2
- Roboguide-3
