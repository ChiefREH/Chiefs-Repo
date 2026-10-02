# EMULATE + CONVERT 4-Way TOF + CTD

## TASKS
1. Emulate in the classroom
2. Convert and deploy in the lab

A 4-way **NORTH-SOUTH/EAST-WEST** traffic pattern using the following LD instructions:
- All necessary **BRANCHES, XIC, XIO, and OTE** instructions
- (3) **TOF** Timers to control the NORTH-SOUTH lights 
- (3) **TOF** Timers to control the EAST-WEST lights 
- (1) **CTD** Counter to control the number of program loops
- (1) **RES** Reset instruction to **manually** reset the CTD from software
> The RES instruction does not require an additional button.


## TIMING
- All **Red** Lights = 10 seconds 
- All **Green** Lights = 7 seconds 
- All **Yellow** Lights = 3 seconds
- Counter = 3 loops

> Refer to the **Traffic Light Output** file in Homebrew for proper output light spacing

## PARAMETERS

- Use a **SEAL-IN** circuit to start/stop the routine
    - _Must alias to wired push-buttons in the lab_
- Routine must continually loop until the Counter is done
- When the Counter is done, the routine must shutdown on its own
- The light sequence must follow the common logical sequence 
    - Do not create a traffic jam or motor vehicle accident!


*Proper rung documentation is mandatory.