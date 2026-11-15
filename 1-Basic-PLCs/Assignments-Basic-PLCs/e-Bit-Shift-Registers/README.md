# BIT SHIFT REGISTERS

Bit Shift Left (BSL) and Bit Shift Right (BSR) instructions are used to move data within a register or array of bits. They are particularly useful for tracking products, sequencing operations, managing outputs, and monitoring machine conditions.

Think of them as moving a series of ON/OFF bits one position at a time.

Common applications:
- Tracking products moving along a conveyor.
- Following a part through multiple manufacturing stations.
- Sequencing machine operations.
- Tracking inspection results.
- Creating a running history of machine events.

## BSL /  BSR Instructions
- Bit Shift Left
- Bit Shift Right


## INSTRUCTION TAGS

- **ARRAY:** The "storage" DINT we are shifting
- **CONTROL:** The control structure for the operation
    - **Length (.LEN):** Number of bits in the array to shift
- **SOURCE BIT:** The bit we shift into the vacated position
    - It's shifting in a "1" or a "0" to the left
    - BSL: Everything shifts to the left!

## LAB

Use the push-button wiring from the previous assignment
- N.O. to set the Source bit to 1/0 (on/off) 
- N.O. to shift the bits through the DINT Array[1] 
