# MPMC-MANUAL



## 

##### EX NO: 1 ## ARITHMETIC OPERATIONS USING 8086 MICROPROCESSORS

> **AIM:** To write and execute Assembly language Program to perform
> arithmetic operations for 8086 microprocessor.
>
> **APPARATUS REQUIRED:** Personal computer with MASM software
>
> **1a)ASSEMBLY LANGUAGE PROGRAM BY DIRECT METHOD FOR ADDITION**
>
> **ALGORITHM:**
>
> **Step 1:** Open command prompt. **Step 2:** Type c: then cd masm â€º
> edit . **Step 3:** Then type the program.
>
> **Step 4:** Initialize the memory location of 1^st^ number.
>
> **Step 5 :** Then increment the content of HL register pair and get
> second data
>
> **Step 6:** Then perform the operation with accumulator and store the
> result in memory location.
>
> **Step 7:** For output,type masm filename.asm,,;
>
> link filename,,; debug filename.exe
>
> **Step 8 :** Stop.

##### PROGRAM:

> CODE SEGMENT
>
> ASSUME CS: CODE,DS:CODE ORG 1000H
>
> MOV CL,00H
> MOV AX,1234H
> MOV BX,1234H
> ADD AX,BX JNC L1
>
> INC CL
>
> L1: MOV SI,1200H MOV \[SI\],AX MOV \[SI+2\],CL MOV AH,4CH INT 21H
>
> CODE ENDS
> END
>
> **OUTPUT FOR ADDITION (DIRECT METHOD):**

+----------------------------------+-----------------------------------+
| > MEMORY LOCATION(INPUT)         | > MEMORY LOCATION(OUTPUT)         |
+==================================+===================================+
|                                  |                                   |
+----------------------------------+-----------------------------------+
|                                  |                                   |
+----------------------------------+-----------------------------------+
|                                  |                                   |
+----------------------------------+-----------------------------------+
|                                  |                                   |
+----------------------------------+-----------------------------------+

Manual calculations:
