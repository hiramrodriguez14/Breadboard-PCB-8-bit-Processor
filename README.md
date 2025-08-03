# 8-Bit TTL SAP-1 Computer

A simple **8-bit SAP-1 style computer** built entirely with **TTL logic chips**, inspired by Ben Eater’s design but redesigned for improved reliability and compactness. This project uses a **Von Neumann architecture**, sharing program and data memory, and is **Turing-complete**. It features a breadboard prototype and a PCB version in development using surface-mount components for a smaller, cheaper, and more robust design.

## Demo Video

[![Demo Video](https://img.youtube.com/vi/YOUR_VIDEO_ID/0.jpg)](https://www.youtube.com/watch?v=YOUR_VIDEO_ID)

*Watch the demo video to see the breadboard computer in action.*

## General Features

- Clock speed up to 500 kHz  
- 8-bit Arithmetic Logic Unit (ALU) capable of addition, subtraction, and software-implemented multiplication and division  
- 4-bit Program Counter (PC) and Memory Address Register (MAR)  
- 32 bytes of memory (shared for program and data) with 8-bit word size  
- Two 8-bit general purpose registers  
- 8-bit data bus  
- Output module with two 4-bit registers to display signed and unsigned values via instructions  
- Control unit implemented with microcode stored in EEPROMs  
- 17 control flags managing internal operations  

## Instruction Set Architecture (ISA)

| Opcode | Mnemonic | Description                            |
|--------|-----------|------------------------------------|
| 0000   | NOP       | No operation                        |
| 0001   | LDA       | Load accumulator from memory       |
| 0010   | ADD       | Add memory to accumulator           |
| 0011   | SUB       | Subtract memory from accumulator    |
| 0100   | OUT       | Output accumulator content          |
| 0101   | JMP       | Jump to address                     |
| 0110   | JC        | Jump if carry                      |
| 0111   | JZ        | Jump if zero                       |
| 1000   | HLT       | Halt the program                    |

*This ISA is based on the classic SAP-1 architecture with Von Neumann shared memory.*

## Breadboard Computer

![Breadboard Computer](./images/breadboard.jpg)

## Schematic

![Schematic](./images/schematic.png)

## Future Plans

- Design and produce a PCB version using surface-mount components to reduce size, cost, and improve reliability  
- Modify and fix design issues found in the breadboard implementation and existing PCB versions  
- Improve layout and routing for better compactness  
- Expand instruction set and add features based on user feedback  

> Note: The PCB design is not made from scratch — the original creator shared the repository, but I’m customizing it to address problems discovered during breadboard assembly and existing PCB designs.

---

Feel free to open issues or submit pull requests if you'd like to contribute!

