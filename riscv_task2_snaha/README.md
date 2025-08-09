RISC-V Task 2 — Local Setup, Assembly, and Instruction Decoding

Introduction
This project demonstrates ability to set up and use a local RISC-V toolchain, compile and run programs on the Spike RISC-V simulator, generate assembly and disassembly outputs, and manually decode RISC-V integer instructions.  
The work includes four C programs (`factorial`, `max_array`, `bitops`, `bubble_sort`), each compiled with unique build identifiers to ensure results are specific to the machine. All outputs, assembly files, and instruction decoding are included in this repository as per the given task requirements.


## 1. Spike Version
Run the command: spike --help (spike we use doesn't include spike -version command in the source code
Output: Spike RISC-V ISA Simulator 1.1.1-dev






2. RISC-V GCC Version

Run the command: riscv64-unknown-elf-gcc -v

Output: gcc version 8.3.0 (SiFive GCC 8.3.0-2019.08.0) 











