# Assembler and x86-64

Something usefull (may become a cheatsheet in the future) about Assembly.

## Operands

Operand can be categorized by 3 types:
- Immediate value
- Register 
- Memory

Memory operands are denoted by square brackets [], with a size directive TYPE PTR before them.

The types include:
- `BYTE`: 1 byte
- `WORD`: 2 byte
- `DWORD`: 4 byte
- `QWORD`: 8 byte

### Noted:
Here is the amount of data that registers in x86 and x86-64 can holds:
|Register|Data|
|---|---|
| **RAX** | 8 bytes (64 bits) |
| **EAX** | 4 bytes (32 bits) |
| **AX** | 2 bytes (16 bits) |
| **AL** | 1 byte  (8 bits), lower part of **AX** |
| **AH** | 1 byte (8 bits), higher part of **AX** |

Example:
- `QWORD PTF [0x8048000]`: 8 bytes of data starting at 0x8048000
- `WORD PTR [rax]`: 2 bytes of data starting from the address saved in the **RAX** register.

# Common operation code (opcode) for assembly:

| Operation Code (opcode) | Description |
| ----------- | ----------- |
| **Data Transfer** |
| `mov` | **Load Value:** Loads an actual value to that address.|
| `lea` | **Load Effectively Value:** Loads a pointer that point to the item.|
| **Arithmetic** |
|`inc`|**Increase:** Increase that operand value by 1.|
|`dec`|**Decrease:** Reduced that operand value by 1.|
|`add`| Add the value of the 2nd operand to the 1st operand.|
|`dec`| Subtracts the amount of 2nd from 1st operand. | 
|**Logical**|
|`and`||



