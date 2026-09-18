# BASIC ROUTINE EDITING (TABLE + POINTER)

## TASK

- Add an EOAT "Pointer" to the J6 flange at proper location and scale
- Add a Fixture "Table21" at proper location and scale
- Record a continuous loop of 4 corner points using the **WORLD** coordinate system
    - Can we reposition points already created?
        - In Lab? Touchup from the TP??
    - Does the path of travel between corner points follow the edge of the table?
        - How can we fix this?
            - Joint > Linear motion type

## PROGRAM SECTIONS

A standard Routine will **always** contain four (4) Sections:

- **!SETUP:** Instructions that run once at start
- **!MAIN:** Instructions that loop continuously
- **!ERRORS:** Alert the operator of faulty conditions
- **!END OF LINE:** When all instructions are complete

>_All programs will be formatted with these four Sections.<br>Future programs of higher complexity may have additional Sections as needed._


## FOCUS

- Use **INST/EDCMD** to format Sections with **REMARKS**
- **SHIFT / RESET / FWD / BWD** to run a program
    - What happens when recording points with SHIFT toggled?
    - What happens when running BWD in the program?
- **HOLD** to stop the routine (or release dead-man switch)
- **STEP** mode for troubleshooting
    - Notice the @ symbol in the program?
- **FCTN > ABORT (ALL)** to kill a program running in the background
- Export your Routine as an .LS file for offline review


## SECTION SPECIFIC

### !SETUP
- **OVERRIDE** = 10% to slow down the speed of the routine

### !MAIN
- **LBL [100]**
- **JMP LBL [100]**

>_Everything in between LBL and JMP LBL will be looped_

### !ERRORS
- **LBL** [900]

### !END OF LINE
- **LBL** [999]



## VIDEO REFERENCE

- Roboguide-2
- Roboguide-3
