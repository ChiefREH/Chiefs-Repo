# COUNTERS

## BASIC COUNTER STRUCTURE

| ELEMENT            | TAG SUFFIX | DATA TYPE |
|--------------------|------------|-----------|
| PRESET             | .PRE       | DINT      |
| ACCUMULATOR        | .ACC       | DINT      |
| ENABLE BIT         | .EN        | BOOL      |
| UP COUNT BIT       | .CU        | BOOL      |
| DOWN COUNT BIT     | .CD        | BOOL      |
| DONE BIT           | .DN        | BOOL      |
| OVERFLOW BIT       | .OV        | BOOL      |
| UNDERFLOW BIT      | .UN        | BOOL      |

## PARAMETERS

- Unlike a timer, the counter will continue to count beyond its preset value
