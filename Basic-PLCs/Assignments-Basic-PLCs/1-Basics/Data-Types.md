# DATA TYPES

| DATA TYPE | SIZE / BITS       | MIN VALUE / LENGTH      | MAX VALUE / LENGTH         |
|-----------|-----------------|------------------------|----------------------------|
| BOOL      | 1               | 0                      | 1                          |
| SINT      | 8               | -128                   | 127                        |
| INT       | 16              | -32,768                | 32,767                     |
| DINT      | 32              | -2,147,483,648         | 2,147,483,647              |
| REAL      | 32              | -3.4028235×10³⁸        | 3.4028235×10³⁸             |
| STRING    | variable        | 0 characters           | 82 characters (default)    |

## Notes

### REAL:
- 32-bit IEEE-754 single-precision floating point
- Can represent very large and very small numbers, including decimals
- Maximum ~3.4028235×10³⁸, minimum ~-3.4028235×10³⁸

### STRING:
- Rockwell / Logix uses STRING[82] by default (max 82 ASCII characters)
- Can be customized to a larger array if needed: STRING[200], etc.