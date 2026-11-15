# SEQUENCER OUTPUT INSTRUCTION

The Sequencer Output (SQO) instruction is used to control a machine through a predefined sequence of operations.

Rather than programming individual rungs for every step of a machine cycle, you can use a sequencer to store a series of output patterns in an array. The PLC then advances through those patterns, applying the appropriate outputs at each step.

Think of it as a programmable step-by-step machine controller.

A simple example: Imagine a conveyor system with four operations:
1. Start conveyor.
2. Stop conveyor at inspection station.
3. Activate inspection device.
4. Activate reject or pass mechanism.
An SQO instruction can manage the output patterns for all four operations.


## INSTRUCTION TAGS:

- **ARRAY:** The "storage" we are pulling from
- **MASK:** Acts as a "filter" for bit positions
- **DEST:** The destination tag you are sending data to
- **CONTROL:**
    - **Length (.LEN):** How many elements in the array
    - **Position (.POS):** Current position in the array 


## NOTE:

Notice how the SQO does not return to 0 when it loops around.
- Can we create some logic to fix this? 
- How convoluted is that logic?
- Do we really need to return to 0 ?

Can you use an INT instead of a DINT for the Array data structure?

## DEMO TASK:

Stack ones in Storage[16]:

```
    0.  skip this element?
    1.  1
    2.  11
    3.  111
    4.  1111
    5.  11111
    6.  111111
    7.  1111111
    8.  11111111
    9.  1111111
    10. 111111
    11. 11111
    12. 1111
    13. 111
    14. 11
    15. 1
```

Use the push-button (N.O.) in lab to cycle through the sequence
