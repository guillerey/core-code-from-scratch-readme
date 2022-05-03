# core-code-from-scratch-readme

# Week 1:

## Week challenges (Tuesday):

### 1. Interpreted And Compiled Programming Languages:
 
#### Compiled Languages:

This languages are converted directly into machine code that the processor can execute result in more
faster and more efficient code. Need to be compilated every time when a change is needed.

#### Interpreted Languages:

This languages needs to be intepreted by a program to read and execute the code, is more slower than
compiled languages but is cross-platform, easier to debug, and test.

### 2. Is Java compiled or interpreted, or both?

A java program is first compiled into bytecode which JRE can understand. ByteCode is then interpreted
by the JVM making it as interpreted language, so yes, Java is both, compiled and interpreted language.


### 3. Pseudocode currency converter

    START
    Currency <-- GET
    Num <-- GET
    ExchangeRate <-- 1 US$ = 0,0000220734 XBT
    Currency * ExchangeRate
    Result <-- ConversionRate
    PRINT Result
    END


## Week challenges (Wednesday)

### 1. Matrix Binary DOB
										
										
1024    512    256      128      64     32      16      8       4       2       1

  1      1      1        1        0      1       1      1       1       1       0    =      1982
										
![image](https://user-images.githubusercontent.com/30531913/162103387-61ee275d-08e0-4098-8ae0-544da5f63535.png)




### 2. MISP


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

              main:
              li $t1, 
              li $v0, 

              add $t2, $t0, $t1

              li $v0, 4
              la $a0 result_message
              syscall

              li $v0, 1
              move $a0, $t2
              syscall


## Week challenges (Thursday) 

1. Print special numbers exercise

	
	for (let i = 0; i <= 101; i += 2)
		console.log(i);


2. Bad Code exercise
3. Bad Code 2 exercise
4. Follow Git Course

\
\



# Week 2:

## Week challenges (Monday)

1. Follow the github course        **Done**
2. Create an account in Codewars   **Done**
3. Read about: if...else           **Done**   
4. Read about: for                 **Done**  
5. Read about: while               **Done** 
6. Read about: functions           **Done** 

## Week challenges (Tuesday)

1. Multiply exercise
2. ASCII Total exercise
3. Char From ASCII Value exercise
4. Binary Addition exercise
5. Student's Final Grade exercise

## Week challenges (Wednesday) 

1. Holiday VIII - Duty Free exercise
2. Twice As Old exercise
3. Valid Spacing exercise
4. Fake Binary exercise

## Week challenges (Thursday)

1. Remove All Exclamation Marks From The End Of Sentence exercise
2. Vowel Remover exercise
3. Rock Paper Scissors! exercise
4. Persistent Bugger exercise

\
\



# Week 3:

## Week challenges (Monday)

1. Who Likes It? exercise
2. Bit Counting exercise
3. Your Order, Please exercise

## Week challenges (Tuesday)

1. Simple Pig Latin exercise
2. Counting Duplicates exercise
3. Decode The Morse Code exercise

## Week challenges (Wednesday)
1. Valid Parentheses exercise
2. Convert String To Camel Case exercise
3. Unique In Order exercise

## Week challenges (Thursday)

1. Fold An Array exercise
2. Encrypt This! exercise
3. Complete your 1st Core Challenge



