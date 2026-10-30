# 3D PRINTER WITH POSITION REGISTER OFFSETS

STUDENT ASSIGNMENT

- Must offset the X, Y and Z coordinates.
- Include logic to prevent exceeding motion at the UPPER LIMIT.
- Must finish in a **SAFE** position away from the "stack."


## OFFSET DIRECTIONS
```text
FIRST:  -X, +Z
SECOND: -Y, +Z
THIRD:  +X, +Z
FOURTH: +Y, +Z
```

## OFFSET PARAMETERS
- **10 loops** for each direction
- **+5 mm** offset per layer in all directions
    - _Soft-coded offset, so we can alter it while running_


## CORNER CODE EXAMPLE

```text
- L P[3] 100% FINE, Offset PR[5]
- L P[4] 100% FINE, Offset PR[5]
- L P[5] 100% FINE, Offset PR[5]
- L P[6] 100% FINE, Offset PR[5]
- L P[3] 100% FINE, Offset PR[5]
```

## NOTE
- This assignment does not require DI, DO, RI, or RO instructions.
- You can use CALLs for each direction, or you can place the entire sequence into a single routine.
- Figure out the basic motion first, then go back and add UALM safety logic last.


## VIDEO REFERENCE

- Assignment-PR-Offsets
