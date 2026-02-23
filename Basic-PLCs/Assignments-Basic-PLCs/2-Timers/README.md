# TIMERS

## TIME ON TIMER (TON)

| ITEM               | TAG SUFFIX | DATA TYPE |
|--------------------|------------|-----------|
| Preset             | .Pre       | DINT      |
| Accumulator        | .ACC       | DINT      |
| Enable bit         | .EN        | BOOL      |
| Timer Timing bit   | .TT        | BOOL      |
| Done bit           | .DN        | BOOL      |

## FIVE PARTS OF A TIMER INSTRUCTION

- .PRE is the preset number (target) we are trying to reach
    - _You enter this number in **milliseconds**_
- .ACC is the accumulator value, keeping track of our progress
- .EN is set to "1" when the timer is **enabled**
- .TT is set to "1" when the timer is **actively** timing
- .DN is set to "1" when the accumulation **equals** the preset
