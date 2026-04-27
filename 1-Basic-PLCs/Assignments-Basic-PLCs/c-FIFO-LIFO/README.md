# FILE LOAD AND UNLOAD

There are 4 types of Load/Unload Operations:
- FIFO Load: _First In, First Out_ (FFL)
- FIFO Unload: _First In, First Out_ (FFU)
- LIFO Load: _Last In, First Out_ (LFL)
- LIFO Unload: _Last In, First Out_ (LFU)

## INSTRUCTION TAGS

FFL
- **SOURCE:** Data to be stored in the FIFO/LIFO
- **FIFO:** Specify the first element of the FIFO/LIFO
- **CONTROL:** The control structure for the operation
    - **Length (.LEN):** Max number of elements in the array
    - **Position (.POS):** Next location (initial values is typically 0)

FFU
- **FIFO:** Specify the first element of the FIFO/LIFO
- **DEST:** Value unloaded from the FIFO/LIFO
- **CONTROL:** Same control as used in the FFL
    - **Length (.LEN):** Max number of elements in the array
    - **Position (.POS):** Next location (initial values is typically 0)
