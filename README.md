# RISC-V Internship program powered by SAMSUNG and VSD
### This RISC-V Internship using VSDSquadron Mini is based on RISC-V architecture and uses open-source tools to teach students about VLSI SoC Design and RISC-V. The instructor and guide for this internship is Kunal Ghosh Sir, Founder of VSD.

# Basic Details

### Name: Risheek G
### College: R V INSTITUTE OF TECHNOLOGY AND MANAGEMENT, Bengalore 560076
### Email ID: rvit22bec021.rvitm@rvei.edu.in
### GitHub Profile: Risheek-G
### LinkedIN Profile: [Risheek G](https://www.linkedin.com/in/risheek-g-642465273/)

</details>

# Task-1

<details>
<summary> Task-1: C based lab screenshots </summary>
<br>

![t1_1](https://github.com/user-attachments/assets/f21b1a07-8321-45ab-922e-eb723353ddeb)

</details>

<details>
<summary> Task-1: RISC-V based lab screenshots </summary>
<br>

![t1_2](https://github.com/user-attachments/assets/23d78bbb-26d6-4604-aee7-d7a9cd8eb4ac)
</details>

# Task 2
<details>
<summary>Spike Simulation for the C program sum1ton.c and object dump's address allocation observation with calculations</summary>
<br>

![1st ](https://github.com/user-attachments/assets/71adfdc3-60cf-43f6-b50d-d5f13c27f6a3)

</details>
<details>
<summary>C based Lab Screenshots- Implementation of Fibonacci sequence upto 20 terms</summary>
<br>
  
 ![2nd](https://github.com/user-attachments/assets/f7168cdc-930e-45ab-b67b-523a83af6de1)
</details>
<details>
<summary>RISC-V based lab screenshots for Spike Simulation of the C program fibo.c and Object dump's address allocation observations</summary>
<br>
  
#### Using -O1 compilation algorithm

![O1](https://github.com/user-attachments/assets/9ccbf616-99d9-49ef-8cda-744382d42d58)

#### Using -Ofast compliation algorithm

![Ofast](https://github.com/user-attachments/assets/bc040f66-deb1-47ea-a4ba-485a17186fb4)

</details>

# Task 3
<details>
<summary>From the riscv-objdump of your application code, identify 15 unique RISC-V instructions.
For those 15 instructions, determine the exact 32-bit instruction code in their respective instruction type formats.</summary>
<br>

 ![Image](https://github.com/user-attachments/assets/3a30a7f2-4067-4784-a5a4-af0e47cf8d41)
 
Instruction 1
Instruction: lui a2, 0x1
Type: U-Type
Opcode: 0110111 (lui)
Destination Register: a2 = x12 → 01100
Immediate: 0x1 → 00000000000000000001 (20 bits)
Overall Encoding:
00000000000000000001 | 01100 | 0110111

Instruction 2
Instruction: lui a0, 0x21
Type: U-Type
Opcode: 0110111 (lui)
Destination Register: a0 = x10 → 01010
Immediate: 0x21 → 00000000000100001 (20 bits)
Overall Encoding:
00000000000100001 | 01010 | 0110111

Instruction 3
Instruction: addi sp, sp, -16
Type: I-Type
Opcode: 0010011 (addi)
Destination Register: sp = x2 → 00010
Source Register: sp = x2 → 00010
Immediate: -16 → 1111111111110000 (12 bits, sign-extended)
Overall Encoding:
1111111111110000 | 00010 | 000 | 00010 | 0010011

Instruction 4
Instruction: addi a2, a2, 954
Type: I-Type
Opcode: 0010011 (addi)
Destination Register: a2 = x12 → 01100
Source Register: a2 = x12 → 01100
Immediate: 954 → 0011101010 (12 bits, sign-extended)
Overall Encoding:
0011101010 | 01100 | 000 | 01100 | 0010011

Instruction 5
Instruction: addi a1, a1, 100
Type: I-Type
Opcode: 0010011 (addi)
Destination Register: a1 = x11 → 01011
Source Register: a1 = x11 → 01011
Immediate: 100 → 00000001100100 (12 bits, sign-extended)
Overall Encoding:
00000001100100 | 01011 | 000 | 01011 | 0010011

Instruction 6
Instruction: addi a0, a0, 384
Type: I-Type
Opcode: 0010011 (addi)
Destination Register: a0 = x10 → 01010
Source Register: a0 = x10 → 01010
Immediate: 384 → 00000110000000 (12 bits, sign-extended)
Overall Encoding:
00000110000000 | 01010 | 000 | 01010 | 0010011

Instruction 7
Instruction: sd ra, 8(sp)
Type: S-Type
Opcode: 0100011 (sd)
Source Register: ra = x1 → 00001
Base Register: sp = x2 → 00010
Immediate: 8 → 0000000001000 (split into imm[11:5] and imm[4:0])
Overall Encoding:
0000000 | 00001 | 00010 | 010 | 0001000 | 0100011

Instruction 8
Instruction: jal ra, 1040c
Type: J-Type
Opcode: 1101111 (jal)
Destination Register: ra = x1 → 00001
Offset: 1040c → 00010000000000001100 (20 bits, sign-extended)
Overall Encoding:
00010000000000001100 | 00001 | 1101111

Instruction 9
Instruction: ld ra, 8(sp)
Type: I-Type
Opcode: 0000011 (ld)
Destination Register: ra = x1 → 00001
Base Register: sp = x2 → 00010
Immediate: 8 → 0000000001000 (12 bits, sign-extended)
Overall Encoding:
0000000001000 | 00010 | 011 | 00001 | 0000011

Instruction 10
Instruction: addi a0, a0, 0
Type: I-Type
Opcode: 0010011 (addi)
Destination Register: a0 = x10 → 01010
Source Register: a0 = x10 → 01010
Immediate: 0 → 000000000000 (12 bits, sign-extended)
Overall Encoding:
000000000000 | 01010 | 000 | 01010 | 0010011

Instruction 11
Instruction: addi sp, sp, 16
Type: I-Type
Opcode: 0010011 (addi)
Destination Register: sp = x2 → 00010
Source Register: sp = x2 → 00010
Immediate: 16 → 00000000010000 (12 bits, sign-extended)
Overall Encoding:
00000000010000 | 00010 | 000 | 00010 | 0010011

Instruction 12
Instruction: ret
Type: I-Type (jalr)
Opcode: 1100111 (jalr)
Destination Register: x0 → 00000
Base Register: ra = x1 → 00001
Immediate: 0 → 000000000000 (12 bits, sign-extended)
Overall Encoding:
000000000000 | 00001 | 000 | 00000 | 1100111
</details>

# Task 4

<details>
<summary>Perform a functional simulation of the given RISC-V Core Verilog netlist and testbench.</summary>
 
## 1. RISC-V RV32I

This project provides an insight into the working of a few important instructions of the instruction set of a Single cycle Reduced Instruction Set Computer - Five(RISC-V) Instruction Set Architecture suitable for use across wide-spectrum of Applications from low power embedded devices to high performance Cloud based Server processors. The base RISC-V is a 32-bit processor with 31 general-purpose registers, so all the instructions are 32-bit long. Some Applications where the RISC-V processors have begun to make some significant threads are in Artificial intelligence and machine learning, Embedded systems, Ultra Low power processing systems etc.

## 2. BLOCK DIAGRAM OF RISC-V RV32I
![image](https://user-images.githubusercontent.com/110079631/181293948-beb8622c-7696-4b06-b6c9-eeab9b8ab9d3.png)

## 3. INSTRUCTION SET OF RISC-V RV32I
![image](https://user-images.githubusercontent.com/110079631/181298133-60269bc2-01da-4b5c-8b42-69057b8dc15c.png)

## 4. FUNCTIONAL SIMULATION

### 4.1 About iverilog and gtkwave
- Icarus Verilog is an implementation of the Verilog hardware description language.
- GTKWave is a fully featured GTK+ v1. 2 based wave viewer for Unix and Win32 which reads Ver Structural Verilog Compiler generated AET files as well as standard Verilog VCD/EVCD files and allows their viewing.

### 4.2 Installing iverilog and gtkwave

- *For Ubuntu*

 Open your terminal and type the following to install iverilog and GTKWave
 
 $   sudo apt get update
 $   sudo apt get install iverilog gtkwave
 

- *To clone the repository and download the netlist files for simulation , enter the following commands in your terminal.*

 
 $ git clone https://github.com/vinayrayapati/iiitb_rv32i
 $ cd iiitb_rv32i
 
- *To simulate and run the verilog code , enter the following commands in your terminal.*


$ iverilog -o iiitb_rv32i iiitb_rv32i.v iiitb_rv32i_tb.v
$ ./iiitb_rv32i

- *To see the output waveform in gtkwave, enter the following commands in your terminal.*

$ gtkwave iiitb_rv32i.vcd

### 4.3 The output waveform
 
 Instruction 1:add r6,r2,r1
 
 ![Image](https://github.com/user-attachments/assets/5f442b64-ca75-4a44-8ed2-4edf395b451d)

 Instruction 2:sub r7,r1,r2
 
![Image](https://github.com/user-attachments/assets/d466f3d7-56bd-4a64-8259-b737a30cc91a)

 Instruction 3:and r8,r1,r3
 
![Image](https://github.com/user-attachments/assets/3e393c85-07df-4f25-bb9a-a256d58ad89a)

 Instruction 4:or r9,r2,r5
 
 ![Image](https://github.com/user-attachments/assets/d32c3e0f-385d-4ea9-8eca-36453c7c536d)

 Instruction 5:xor r10,r1,r4
 
![Image](https://github.com/user-attachments/assets/448bc592-c25c-4819-a5fb-26d67066549a)

 Instruction 6:slt r11,r2,r4
 
 ![Image](https://github.com/user-attachments/assets/db820b84-7ba8-4025-9aac-085f7c4232a4)

 Instruction 7:addi r12,r4,5
 
 ![Image](https://github.com/user-attachments/assets/26e1c82e-e76d-43d6-9e55-918d1268fb21)

 Instruction 8:sw r3,r1,2
 
 ![Image](https://github.com/user-attachments/assets/e9a439af-6861-4c2d-b781-7666bc3abfb3)

 Instruction 9:lw r13,r1,2
 
 ![Image](https://github.com/user-attachments/assets/afe41c20-05da-4e39-a88f-dfa03e038afa)

 Instruction 10:beq r0,r0,15
 
 ![image](https://github.com/user-attachments/assets/1afe2bb4-5055-4958-913b-f9719ed5b40c)

</details>

# Task 5

<details>
<summary> PDF containing explaination of project idea </summary>
 
  [VSDSquadron Project.pdf](https://github.com/user-attachments/files/18832582/VSDSquadron.Project.pdf)

</details>

# Task 6


 <summary>The codes, the output screenshots, and the video of setup is in the Task6 file 
 </summary>
