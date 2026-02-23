# BASIC BITS

## TAGS

- Think of tags as human readable "nicknames" for tiny sections of PLC memory
- We store 1s and 0s in these tiny sections of memory
- The instructions tell the PLC **what** to look for, and **where** to look for it
    - Basic input instructions (XIC, XIO) look for 1s and 0s at the assigned tag (memory) location
    - Based on what is stored at the location, the instruction generates a true/false signal for the output instruction (OTE)


## TRUTH TABLE

- XIC sends a true signal on 1, false signal on 0
- XIO sends a true signal on 0, false signal on 1
- OTE is 1 if continuity is true, 0 if continuity is false*

> _*OTL -( L )- and OTU -( U )- break this logic_


## Simple boolean AND statement

- Reading left to right on the ladder rung:
    - If there is a 0 at address "Tag_2"
        - And
    - There is a 1 at address "Tag_1"
        - THEN
    - OTE will write a 1 to address "Tag_3"

> _This is a boolean expression of an AND statement_

```text
L      Tag_2        Tag_1        Tag_3      R
|------[ / ]--------[   ]--------(   )------|

-[   ]- XIC
-[ / ]- XIO
-(   )- OTE

```

## Simple boolean OR statement

- Reading left to right on the ladder rung:
    - If there is a 0 at address "Tag_2"
    - And there is a 1 at address "Tag_1"
        - OR
    - There is a 0 at address "Tag_2"
    - And there is a 1 at address "Tag_4"
        - THEN
    - OTE will write a 1 to address "Tag_3"

> _This is a boolean expression of an OR statement_

```text
L      Tag_2        Tag_1       Tag_3      R
|------[ / ]----+---[   ]---+---(   )------|
                |           |
                |   Tag_4   |
                |---[   ]---|

-[   ]- XIC
-[ / ]- XIO
-(   )- OTE

```

