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


## Simple IF - THEN statement (SERIES)

- Moving left to right on the ladder rung:
    - If there is a 1 at address "Tag_1"
        - THEN
    - OTE will write a 1 to address "Tag_2"

> _This is a boolean expression of an AND statement_

```text
L         Tag_1            Tag_2         R
|---------[   ]------------(   )---------|


-[   ]- XIC
-[ / ]- XIO
-(   )- OTE

```


## Simple boolean AND statement (SERIES)

- Moving left to right on the ladder rung:
    - If there is a 1 at address "Tag_1"
        - And
    - If there is a 1 at address "Tag_2"
        - THEN
    - OTE will write a 1 to address "Tag_3"

> _This is a boolean expression of an AND statement_

```text
L      Tag_1        Tag_2        Tag_3      R
|------[   ]--------[   ]--------(   )------|


-[   ]- XIC
-[ / ]- XIO
-(   )- OTE

```

## Simple boolean OR statement (PARALLEL)

- Moving left to right on the ladder rung:
    - If there is a 1 at address "Tag_1"
        - OR
    - If there is a 1 at address "Tag_2"
        - THEN
    - OTE will write a 1 to address "Tag_3"

> _This is a boolean expression of an OR statement_

```text
L         Tag_1             Tag_3      R
|-----+---[   ]---+---------(   )------|
      |           |
      |   Tag_2   |
      |---[   ]---|


-[   ]- XIC
-[ / ]- XIO
-(   )- OTE

```

## Simple AND - OR statement (COMBO)

- Moving left to right on the ladder rung:
    - If there is a 1 at address "Tag_1"
        - AND
    - If there is a 1 at address "Tag_2"
        - OR
    - If there is a 1 at address "Tag_3"
        - THEN
    - OTE will write a 1 to address "Tag_4"

```text
L      Tag_1           Tag_2             Tag_4      R
|------[   ]-------+---[   ]---+---------(   )------|
                   |           |
                   |   Tag_3   |
                   |---[   ]---|


-[   ]- XIC
-[ / ]- XIO
-(   )- OTE

```

## Simple Seal-In Circuit for Motor Control

QUESTION
- _How does this combo differ from the previous examples?_
- _Why configure the ladder in this way?_

```text
L      Tag_1           Tag_2             Tag_4      R
|------[ / ]-------+---[   ]---+---------(   )------|
                   |           |
                   |   Tag_4   |
                   |---[   ]---|


-[   ]- XIC
-[ / ]- XIO
-(   )- OTE

```
