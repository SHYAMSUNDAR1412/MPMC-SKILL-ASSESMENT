# SKILL ASSESMENT 2 

## Write an assembly language program in 8051 to generate a 50 ms delay using Timer 0 in Mode 2 (8-bit auto-reload mode) and blink an LED connected to Port

AIM:
  To Write an assembly language program in 8051 to generate a 50 ms delay using Timer 0 in Mode 2 (8-bit auto-reload mode) and blink an LED connected to Port

APPARATUS REQUIRED:
   Laptop With Keil Software

PROGRAM:
```
ORG 0000H
MAIN:
    MOV TMOD, #02H
    MOV TH0, #06H
    SETB TR0

LOOP:
    JNB TF0, LOOP
    CPL P3.0
    CLR TF0
    SJMP LOOP
END
```

OUTPUT:
<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/85e9e6c9-710d-46cf-a07e-69108135ba22" />

RESULT:
     Thus,an assembly language program in 8051 to generate a 50 ms delay using Timer 0 in Mode 2 (8-bit auto-reload mode) and blink an LED connected to Port
