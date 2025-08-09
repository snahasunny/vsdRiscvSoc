 RISC-V Integer Instruction Decoding

| Instruction     | Opcode  | rd      | rs1     | rs2     | funct3 | funct7  | Binary (32-bit)                       | Description                                                     |
| --------------- | ------- | ------- | ------- | ------- | ------ | ------- | ------------------------------------- | --------------------------------------------------------------- |
| addi sp,sp,-32  | 0010011 | sp(x2)  | sp(x2)  | ---     | 000    | ---     | 111111111100 00010 000 00010 0010011  | Add immediate -32 to sp and store the result in sp              |
| sd ra,24(sp)    | 0100011 | ---     | sp(x2)  | ra(x1)  | 011    | 0000000 | 0000000 00001 00010 011 11000 0100011 | Store the contents of ra into memory at address sp + 24         |
| mv a0,a5        | 0110011 | a0(x10) | a5(x15) | x0      | 000    | 0000000 | 0000000 00000 01111 000 01010 0110011 | Copy the contents of a5 into a0                                 |
| lw a5,-20(s0)   | 0000011 | a5(x15) | s0(x8)  | ---     | 010    | ---     | 1111111111000 01000 010 01111 0000011 | Load a 32-bit word from memory at address s0 - 20 into a5       |
| and a5,a5,a4    | 0110011 | a5(x15) | a5(x15) | a4(x14) | 111    | 0000000 | 0000000 01110 01111 111 01111 0110011 | Perform bitwise AND between a5 and a4; store result in a5       |
| or a5,a5,a4     | 0110011 | a5(x15) | a5(x15) | a4(x14) | 110    | 0000000 | 0000000 01110 01111 110 01111 0110011 | Perform bitwise OR between a5 and a4; store result in a5        |
| xor a5,a5,a4    | 0110011 | a5(x15) | a5(x15) | a4(x14) | 100    | 0000000 | 0000000 01110 01111 100 01111 0110011 | Perform bitwise XOR between a5 and a4; store result in a5       |
| slliw a5,a5,0x3 | 0011011 | a5(x15) | a5(x15) | ---     | 001    | 0000000 | 0000000 00011 01111 001 01111 0011011 | Shift a5 left logically by 3 bits (32-bit result); store in a5  |
| srliw a5,a5,0x2 | 0011011 | a5(x15) | a5(x15) | ---     | 101    | 0000000 | 0000000 00010 01111 101 01111 0011011 | Shift a5 right logically by 2 bits (32-bit result); store in a5 |
| add a5,a5,a4    | 0110011 | a5(x15) | a5(x15) | a4(x14) | 000    | 0000000 | 0000000 01110 01111 000 01111 0110011 | Add the values of a5 and a4; store the result in a5             |

