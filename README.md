# core-code-from-scratch-readme

1.
Interpreted And Compiled Programming Languages:
----------------------------------------------------

Compiled Languages:
---------------------
This languages are converted directly into machine code that the processor can execute result in more
faster and more efficient code. Need to be compilated every time when a change is needed.

Interpreted Languages:
------------------------
This languages needs to be intepreted by a program to read and execute the code, is more slower than
compiled languages but is cross-platform, easier to debug, and test.

2.
Is Java compiled or interpreted, or both?
---------------------------------------------

A java program is first compiled into bytecode which JRE can understand. ByteCode is then interpreted
by the JVM making it as interpreted language, so yes, Java is both, compiled and interpreted language.


3.
Pseudocode currency converter
-------------------------------

START
Currency <-- GET
Num <-- GET
ExchangeRate <-- 1 US$ = 0,0000220734 XBT
Currency * ExchangeRate
Result <-- ConversionRate
PRINT Result
END


Week challenges (Wednesday)
----------------------------

Matrix Binary DOB
										
										
1024	512	256	128	64	32	16	8	4	2	1

1	1	1	1	0	1	1	1	1	1	0    =      1982
										
![image](https://user-images.githubusercontent.com/30531913/162103387-61ee275d-08e0-4098-8ae0-544da5f63535.png)




MISP
-----


.data
	      number1: .asciiz "\nIngrese el primer numero: "
	      number2: .asciiz "\nIngrese el segundo numero: "
	      result_message: .asciiz "\nEl resultado es: "

  .text
	      main:
              li $v0, 4
              la $a0, number1
              syscall

              li $v0, 5
              syscall

              move $t0, $v0

              li $v0, 4
              la $a0, number2
              syscall

              li $v0, 5
              syscall

              move $t1, $v0

              li $v0, 1
              move $a0, $t0
              syscall

              li $t1, 0
              li $v0, 100
 
              add $t1, $a0, $t1

              li $v0, 4
              la $a0 result_message
              syscall

              li $v0, 1
              move $a0, $t0
              syscall




