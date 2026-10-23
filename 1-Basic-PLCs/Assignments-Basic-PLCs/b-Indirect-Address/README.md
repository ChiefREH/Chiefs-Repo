# INDIRECT ADDRESSING

- Substitute a hard-coded value with a **CTU.ACC**
- Hard Coding vs Soft Coding
    - _Similar to Registers **R[ ]** in Robotics_
- There are dangers when writing to arrays that don't exist
    - **Major Faults** will arise if you try to move data to an Array that does not exist!


## DEMO: MANUAL PUSH

- Create a DINT[3]
- Using INDIRECT ADDRESSING, manually "push" these numbers to the Array:
    - DINT[0]: 123
    - DINT[1]: 456
    - DINT[2]: 789



## DEMO: MANUAL PULL

- Create a DINT[3]
- Store these numbers in the Array:
    - DINT[0]: 123
    - DINT[1]: 456
    - DINT[2]: 789

- Using INDIRECT ADDRESSING, manually "pull" one value at a time and move it to the output module.
