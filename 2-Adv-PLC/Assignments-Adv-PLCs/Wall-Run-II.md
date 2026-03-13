# WALL RUN II


## HMI SEQUENCE:

- Flash individual screens from dark > bright > dark, down the wall and back again (“bounce”)
    - bright interval: 0.5 seconds
- Fill and clear screens in sequence, down and back (“snake”)
    - 1.0 second interval
- Flash individual letters on each screen, down and back
    - 2.0 second interval (_adjust for best effect_)
    - Letters must be scaled up as large as possible
        - _Use the same font for each; don't mix and match!_
- Flash the entire phrase on/off
    - _repeat 3 times_
- Start sequence again


## PARAMETERS:

- Can use Prod/Con tags or MSG instruction (all global/controller scope)
    - _Don’t even attempt to “synchronize” the operation using TON/TOF timers_
- Use Properties, State Tables and/or Color Tables, as needed
- Must have 1 start/stop screen only (at the far end of the lab)
- Must use all PLC/HMI combos
    - _if wiring is required, power down the equipment and make it happen!_
