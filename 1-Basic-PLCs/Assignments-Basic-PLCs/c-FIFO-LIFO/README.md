# FILE LOAD AND UNLOAD

FIFO and LIFO instructions are used to store, organize, and retrieve data in a specific order.

They are particularly useful in industrial automation when a PLC needs to remember information about products, machine operations, or production events and retrieve that information later.

There are four primary instructions in Studio 5000:

| Instruction | Full Name   | Function                 |
| ----------- | ----------- | ------------------------ |
| **FFL**     | FIFO Load   | Adds data to a FIFO      |
| **FFU**     | FIFO Unload | Removes data from a FIFO |
| **LFL**     | LIFO Load   | Adds data to a LIFO      |
| **LFU**     | LIFO Unload | Removes data from a LIFO |

The difference is the order in which information is retrieved.

## RETRIEVAL ORDER

- FIFO: First In, First Out
- LIFO: Last In, First Out


## INSTRUCTION TAGS

FFL (FIFO Load)
- **SOURCE:** Data to be stored in the FIFO/LIFO
- **FIFO:** Specify the first element of the FIFO/LIFO
- **CONTROL:** The control structure for the operation
    - **Length (.LEN):** Max number of elements in the array
    - **Position (.POS):** Next location (initial value is typically 0)

FFU (FIFO Unload)
- **FIFO:** Specify the first element of the FIFO/LIFO
- **DEST:** Value unloaded from the FIFO/LIFO
- **CONTROL:** Same control as used in the FFL
    - **Length (.LEN):** Max number of elements in the array
    - **Position (.POS):** Next location (initial value is typically 0)
