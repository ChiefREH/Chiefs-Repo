# STUDIO 5000 EMULATOR SETUP

**REMEMBER:**  Right-click all and run as Administrator

Get your IP Address > <u>Command Prompt</u> > type _ipconfig_ > keep this handy, you’ll need it later.

## Open RSLinks Classic
- Set up Rslinx Drivers:  Open <u>RSLinx</u> > Configure Drivers > select from the dropdown:
    - AB-ETHIP - give it a unique name that you’ll recognize
    - AB-VBP - give it a unique name that you’ll recognize
        - Stop any other drivers that may be running to prevent conflicts!

## Setup Studio 5000 Logix Emulate (virtual chassis):
- Slot 0: RSLinx Classic for communications  (_might be in a different slot on your machine_)
- Slot 1: FatoryTalk Linx for communications  (_might be in a different slot on your machine_)
- Slot 2: Right-click > Create > Emulate 5570 Controller
    - Confirm the version matches the version of Logix Designer software we use.
    - Accept the rest of the default settings as-is.

### Add virtual Input/Output (I/O) Modules:
- Slot 3: Right-click > Create > 1756-SIM 32 Point Input/Output Simulator
- Label for marquee:  INPUTS
- Slot 4: Right-click > Create > 1756-SIM 32 Point Input/Output Simulator
- Label for marquee:  OUTPUTS

## Launch Studio 5000 > New Project
- Left-hand Column:  Logix
- Dropdown Menu:  Studio 5000 Logix Emulate Controller > Emulate 5570 Studio 5000 Logix Emulate Controller
- Name:  Emulated_Project_add_your_initials_to_the_end
- Version:  Confirm same as earlier (v34 for this semester?)
- Chassis:  1756-A10 10-Slot ControlLogix Chassis
    - _I prefer the A17 17-slot chassis_
- Slot:  Must match the slot established in Studio 5000 Logix Emulate (virtual chassis)
- Click Finish

## Logix Designer Overview:
- Faceplate: Different modes of operation and controller properties
- Controller Organizer Window (COW):  all the tasks, programs and routines
    - Check Controller Tags (near top):  _Are there any tags listed?_

### I/O Configuration: 
- Add in the virtual hardware for the program to interact with:
    - Right-click Backplane > New Module > Select Module Type dialog box > Catalog tab
    - Deselect Module Type filter > Scroll Down > Select the “Other” category
    - Select 1756-MODULE “Generic 1756 Module” > click Create
    - New Module Dialog:  Name: Simulated_Inputs
    - Slot:  Matches our Studio 5000 Logix Emulate virtual chassis Slot 3

![Module COnnection Parameters](Homebrew-Basic-PLC-Images/Module-Connx-Parameters.png)

### Connection Parameters:
- Input 1 | 2
- Output 2 | 1
- Configuration 16 | 0

### Module Properties Report dialog box:
- Requested Packet Interval (RPI):  must be changed to 50ms.
    - _See “Getting Good Results” page 30 for the Tip at the top._
- Click Apply + OK

## REPEAT THE INPUT STEPS ABOVE FOR THE OUTPUT MODULE
- Change Name to Simulated_Outputs
- Slot:  Matches our Studio 5000 Logix Emulate virtual chassis Slot 4
- Same Configuration Parameters as picture (1|2, 2|1, 16|0)
- Requested Packet Interval (RPI):  must be changed to 50ms.
- _See “Getting Good Results” page 30 for the Tip at the top._
- Click Apply + OK

> Emulator and I/O are now configured. Go back to Controller Tags section:  Are there tags now?

## I/O Addressing Example (Words):
- Expand Local:3:I.Data
- Gives you 2 choices:  Local:3:I.Data[0] and Local:3:I.Data[1]
- **We want to use Local:3:I.Data[1]**
    - For Output > only gives on option > Local:4:O.Data[0]

## EXERCISE: Manipulate The Simulated Chassis Input Bits
- Studio 5000 Logix Emulate Virtual Chassis > Right-click Input module > Properties > I/O Data tab 
- Dialog box showing all inputs and outputs for that Slot > Leave on screen so we can input On/Off
- Can see Logix changing the On/Off in real-time
	Repeat for Output card

## Selecting a Controller Path for the Project:
- In Logix > RSWho > Navigate to the VBP that you created at YOUR IP ADDRESS
    - **Do Not use another VBP on the RSLinx Network!**
- In View Designer > Navigate to the ETHIP that you created at YOUR IP ADDRESS
    - Do Not use another ETHIP on the RSLinx Network!