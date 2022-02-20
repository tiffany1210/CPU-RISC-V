# CPU-RISC-V
CS61C project 3 CPU

This project specification uses python3 for sample commands; depending on your system, you may need to use python or py instead. It uses Logisim Evolution, a Java-based GUI program.

***Arithmetic Logic Unit (ALU)***
- I created an ALU that supports all the operations needed by the instructions in our ISA. 
Below is the list of ALU operations I implemented, along with their associated ALUSel values.

![Screen Shot 2022-02-20 at 12 00 04 AM](https://user-images.githubusercontent.com/47617094/154833900-e86ec3c8-dc5c-4b29-89ce-f0d1d0a16626.png)

***Register File (RegFile)***
 - RegFile writes / reads from registers specified in a given RISC-V instruction without affecting any other registers. There is one notable exception: RegFile should NOT write to x0, even if an instruction tries. The zero register should ALWAYS have the value 0x0. 
 - The register file circuit has six inputs:
 
 ![Screen Shot 2022-02-20 at 12 07 00 AM](https://user-images.githubusercontent.com/47617094/154834082-b5c7941f-9cc7-4c97-a3e3-da1727bd9347.png)
- The register file also has the following outputs:
- 
![Screen Shot 2022-02-20 at 12 07 37 AM](https://user-images.githubusercontent.com/47617094/154834106-a20abcf3-7381-4067-a18f-34584d5097a6.png)


 
 ***The addi Instruction***
 - Memory:
 
![Screen Shot 2022-02-20 at 12 07 51 AM](https://user-images.githubusercontent.com/47617094/154834125-2f1afc0f-ed02-458d-a74b-abe3971aefe3.png)

- Branch Comparator:

![Screen Shot 2022-02-20 at 12 09 00 AM](https://user-images.githubusercontent.com/47617094/154834160-04f32217-5125-4aae-affc-d6b758126aec.png)

-  Immediate Generator:

![Screen Shot 2022-02-20 at 12 09 55 AM](https://user-images.githubusercontent.com/47617094/154834187-47a1b0ba-5eef-4daf-be8f-4cb64146510e.png)

-  Processor:

![Screen Shot 2022-02-20 at 12 10 03 AM](https://user-images.githubusercontent.com/47617094/154834191-de099a58-b619-48b1-a6f2-5a6f05027d63.png)

![Screen Shot 2022-02-20 at 12 10 11 AM](https://user-images.githubusercontent.com/47617094/154834194-26eba937-d8fb-4592-8df6-03ce03161bb5.png)


-  Control Logic

- Pipelining Your CPU
