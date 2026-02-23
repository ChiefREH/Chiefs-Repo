# BASIC BITS

## TRUTH TABLE

- XIC is true on 1, false on 0
- XIO is true on 0, false on 1
- OTE is 1 if continuity is true*

> _*OTL and OTU break this logic_


## SIMPLE LADDER DIAGRAM

- Reading left to right on the ladder rung:
    - If there is a 0 at address "Tag_2"
    - And if there is a 1 at address "Tag_1"
    - OTE will write a 1 to address "Tag_3"

> _This is a boolean AND statement_

```text
+      Tag_2        Tag_1        Tag_3      -
|------[ / ]--------[   ]--------(   )------|

-[   ]- XIC
-[ / ]- XIO
-(   )- OTE

```
