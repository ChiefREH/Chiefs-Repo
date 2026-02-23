# BASIC BITS

## TRUTH TABLE

- XIC is true on 1, false on 0
- XIO is true on 0, false on 1
- OTE is 1 if continuity is true, 0 if false*

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
