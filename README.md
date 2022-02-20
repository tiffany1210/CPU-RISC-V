# CPU-RISC-V
CS61C project 3 CPU

This project specification uses python3 for sample commands; depending on your system, you may need to use python or py instead. It uses Logisim Evolution, a Java-based GUI program.

***Arithmetic Logic Unit (ALU)***
- I created an ALU that supports all the operations needed by the instructions in our ISA. 
Below is the list of ALU operations I implemented, along with their associated ALUSel values.

![Screen Shot 2022-02-20 at 12 00 04 AM](https://user-images.githubusercontent.com/47617094/154833900-e86ec3c8-dc5c-4b29-89ce-f0d1d0a16626.png)

***Register File (RegFile)***
 - RegFile writes / reads from registers specified in a given RISC-V instruction without affecting any other registers. There is one notable exception: RegFile should NOT write to x0, even if an instruction tries. The zero register should ALWAYS have the value 0x0. 
 
 ***The addi Instruction***
 - Memory
- Branch Comparator
-  Immediate Generator
-  Processor
-  Control Logic

- Pipelining Your CPU
