
# MPMC-SKILL-ASSESSMENT-1

## Write an assembly language program in 8051 to calculate the sum of 5 numbers stored sequentially in memory and store the result in a another memory location.

AIM:
    To Write an assembly language program in 8051 to calculate the sum of 5 numbers stored sequentially in memory and store the result in a another memory location.
    
APPARATUS REQUIRED:
  Laptop With Keil Software

PROGRAM:
```
ORG 0000H       
MOV R0, #30H    
MOV R1, #05    
CLR A       
LOOP: 
    ADD A, @R0   
    INC R0       
    DJNZ R1, LOOP 
MOV 35H, A     
SJMP $    
END
```
OUTPUT:
<img width="1920" height="1140" alt="Screenshot 2025-10-25 123832" src="https://github.com/user-attachments/assets/a48be242-48be-495b-a5b0-6e1baef56005" />

<img width="1920" height="1140" alt="Screenshot 2025-10-25 124002" src="https://github.com/user-attachments/assets/98cb8747-e0d6-4fcd-a2b6-0e4271396a68" />


RESULT:
THUS,the sum of 5 numbers stored sequentially in memory and stored the result in a another memory location.
