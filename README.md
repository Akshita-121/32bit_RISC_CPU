# 32bit_RISC_CPU
The project emphasizes understanding RISC-based microarchitecture, memory management, and instruction decoding principles by building a 32-bit ARM-like CPU
## CPU Instruction Set
This project implements a 32-bit ARM-like CPU capable of handling fundamental RISC-based operations. The CPU supports:

Data Processing Instructions: ADD, SUB, AND, ORR

Memory Operations: STR, LDR

Branch Operation: B

Also, cover all the conditional mnemonics from ARM LRM, as shown in the snapshot below. 

![WhatsApp Image 2024-10-21 at 8 50 46 PM](https://github.com/user-attachments/assets/5dfd10a9-aad9-4771-a08e-51e941b20dde)
ref: Digital Design and Computer Architecture ARM edition by Harris
## Design Flowchart
![CONTROLLER](https://github.com/user-attachments/assets/af8c3444-c097-40d7-aa3c-296017905a7e)
## Main blocks of design (Top View)
![CONTROLLER (3)](https://github.com/user-attachments/assets/d329d7ee-3496-4353-905c-4a43f0584861)
## Dataflow path schematic (Datapath + memory blocks)
![CONTROLLER (2)](https://github.com/user-attachments/assets/e8464267-8cd6-434e-b5b8-27710df71fb6)

## Testing : 

To test a CPU working we need to have an extensive code which can examine each and every instruction covered in this CPU design , and then if that code is being executed by our CPU 
with the required final result we can say that CPU passed the initial test 

To test our design, we have taken reference test Code from Digital Design and Computer Architecture ARM edition by Harris. 

### Test Code : 

![image](https://github.com/user-attachments/assets/6597a10c-7191-4b00-bbf0-d3e907aeeedd)


imem.v : instruction memory source this codes in hexadecimal format . 

testbench.sv : Check if we are getting mem[84]==7 or not, which is the final expected outcome of this test code . 

