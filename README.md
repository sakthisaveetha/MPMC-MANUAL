## ARITHMETIC OPERATIONS USING 8086 MICROPROCESSORS

## 

##### EX NO: 1 DATE:

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
> MOV CL,00H MOV AX,1234H MOV BX,1234H ADD AX,BX JNC L1
>
> INC CL
>
> L1: MOV SI,1200H MOV \[SI\],AX MOV \[SI+2\],CL MOV AH,4CH INT 21H
>
> CODE ENDS END
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

##### Manual calculations:

![](media/image1.png){width="7.388888888888889in"
height="10.516666666666667in"}

> ![](media/image3.png){width="2.45411854768154in"
> height="8.333541119860017in"}
>
> **1b)ASSEMBLY LANGUAGE PROGRAM BY INDIRECT METHOD FOR ADDITION**

#### ALGORITHM:

> **Step 1 :** Initialize the memory location for 1^st^ data in HL
> register.
>
> **Step 2 :** Store 1^st^ data in memory location.
>
> **Step 3 :** Increment the content of HL register for entering data in
> memory location.
>
> **Step 4 :** Store second data in memory location.
>
> **Step 5 :** Move 2^nd^ number in accumulator.
>
> **Step 6 :** Decrease the content of HL register pair.
>
> **Step 7 :** Add the content of memory with accumulator.
>
> **Step 8 :** Store the result in memory location.
>
> **Step 9 :** Stop.

##### ASSEMBLY LANGUAGE PROGRAM :

> **OUTPUT FOR ADDITION (INDIRECT METHOD):**

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

##### Manual calculations:

