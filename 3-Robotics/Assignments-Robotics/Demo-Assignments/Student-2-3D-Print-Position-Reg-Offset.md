# 3D PRINTER WITH POSITION REGISTER OFFSETS

STUDENT ASSIGNMENT

- Must offset the X, Y and Z coordinates.
- Include logic to prevent exceeding motion at the UPPER LIMIT.
- Must finish in a SAFE position away from the "stack."


## OFFSET DIRECTIONS
```
FIRST:  -X, +Z
SECOND: -Y, +Z
THIRD:  +X, +Z
FOURTH: +Y, +Z
```

## OFFSET PARAMETERS
- **10 loops** for each direction
- **+5 mm** offset per layer in all directions
    - _Soft-coded offset, so we can alter it while running_


## NOTE
- This assignment does not require DI, DO, RI, or RO instructions.

## VIDEO REFERENCE

- Assignment-PR-Offsets
