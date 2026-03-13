# TIMERS

## BASIC TIMER STRUCTURE

| ELEMENT            | TAG SUFFIX | DATA TYPE |
|--------------------|------------|-----------|
| PRESET             | .PRE       | DINT      |
| ACCUMULATOR        | .ACC       | DINT      |
| ENABLE BIT         | .EN        | BOOL      |
| TIMER TIMING BIT   | .TT        | BOOL      |
| DONE BIT           | .DN        | BOOL      |


## FIVE PARTS OF A TIMER INSTRUCTION

- .PRE is the preset number (target) we are trying to reach
    - _You enter this number in **milliseconds**_
- .ACC is the accumulator value, keeping track of our progress
- .EN is set to "1" when the timer is **enabled**
- .TT is set to "1" when the timer is **actively** timing
- .DN is set to "1" when the accumulation **equals** the preset
    - _When they are equal, the timer stops timing_
