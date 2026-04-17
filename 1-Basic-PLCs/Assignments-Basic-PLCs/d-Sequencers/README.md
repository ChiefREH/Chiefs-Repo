# SEQUENCER OUTPUT INSTRUCTION

Notice how the SQO does not return to 0 when it loops around.
- Can we create some logic to fix this? 
- How convoluted is that logic?
- Do we really need to return to 0 ?

Can you use an INT instead of a DINT for the Array data structure?

## DEMONSTRATION:

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
