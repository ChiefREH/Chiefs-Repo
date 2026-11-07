# MOVING DATA

- MOV can move data from a one tag to another
    - Original data is not destroyed, only copied
- COP can move multiple elements of a tag
    - Useful when dealing with arrays
- MVM uses a "mask" to filter out certain bits from Source to Destination
    - _we will always set this tag to "-1"_
- CLR will clear all the bits from the Destination tag
- COP will copy a source to the destination Array with a specified length
- FLL will fill a destination with a source value (like all 0s)
- RADIX is the style that information is displayed:
    - Decimal format
    - Binary format
    - Octal format
    - Hex format
    - ASCII format
