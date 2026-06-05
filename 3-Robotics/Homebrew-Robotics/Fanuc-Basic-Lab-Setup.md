# COMMON FANUC LAB ISSUES

Common problems when working with live robots in the lab.

## READY POSITION

- Before any programming takes place, jog/rotate the J5 axis to **-90 degrees** (pointing straight down at the work area).
- This will reduce the chances of a **singularity** during operation.
- Also a good idea to store this new position in a **POSITION REGISTER [PR]**.


## COMMON START-UP PROBLEMS IN LAB

- If you need to **CONFIRM PAYLOAD** [F2] after start-up, enter the Master Code (ask your Instructor)
    - _This sometimes happens with the CR-7_
- If **APPLY DCS PARAM** alarm is active, then:
    - MENU > SYSTEM > DCS > [APPLY] > enter code > [OK]
- When directed to **“cycle power”** after applying DCS, manually turn off the power, wait 15-20 seconds and then turn power back on.
- You can disable the **ETH/IP** alarm from:
    - Menu > I/O menu > last menu on the far right (right arrow x2) > EtherNet/IP > ENTER > the first entry is TRUE > change to FALSE
- Alarm **MCTL-013** can be disabled from:
    - Menu > System > Variable > $OP_WORK > ENTER > set UOP Disable = 1 (TRUE) > ENTER
- If you get a blank screen at start-up, perform an **INIT START** with Instructor guidance.
