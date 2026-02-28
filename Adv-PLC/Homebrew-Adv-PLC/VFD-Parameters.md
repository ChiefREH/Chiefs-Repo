# VFD + MSG PARAMETERS

PowerFlex 525 Quick Start PDF:
[PF525-Quick-Start](https://literature.rockwellautomation.com/idc/groups/literature/documents/qs/520-qs001_-en-e.pdf)

## PARAMETERS:
- Proper VFD pathway configuration
- use "169.169.169.xx7" for the VFD ETH/IP Address
    - Example: 169.169.169.27, 37, 47, 57, 67, etc.
- Proper I/O module selection
- Properly configured VFD tags for:
    - Frequency
    - Voltage
    - Amperage
        - May need a MSG instruction the pull a "Single Attribute" value
            - Refer to the PF525 DeviceNet PDF, pages 56-57
 
## PROJECT NOTES:
- MANUALLY input the VFD's IP address (C128-C136) first
- Then add the 525 EMBEDDED ETHERNET VFD module to the PLC project
- In the VFD Properties Wizard:
    - POWER: 0.75kW / 1.0HP
    - INPUT: 3-phase, 200-240V @ 47-63Hz
    - FRN: 5.001
    - SERIES: A
    - Add check-marks to the Physical Parameters column when prompted.
    - We won't use "Project" because one doesn't exist yet
 
## MSG INSTRUCTION DETAILS:
- Message Type: CIP Generic
- Service Type: Get Attribute Single
    - Service Code: e
    - Class: 93
    - Instance: 1 (frequency) or 3 (current) or 4 (voltage)
    - Attribute: 9
- Tags must be CONTROLLER scoped
- When dividing values, destination tag must be a REAL data type
- IIRC, to start and stop the VFD you must:
    - Send a "1" to the correct Tag to Start the VFD.
    - Then send a "0" to clear the Tag or the Stop won't work.
    - Send a "1" to the correct Tag to Stop the VFD.
    - Send a "0" to clear the Tag or the Start won't work again.

## Note
- If necessary, use Math instructions to multiply by 100 for the correct numerical readout
