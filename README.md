## Week challenges (Tuesday) 💻
### 1.Search and answer the question: Java language is compiled or interpreted?
Java is considered both since it is first compiled into binary code and then the code runs in the Java VM which is usually software-based
### 2. Create an algorithm to calculate the equivalent of your local currencty to USD
```
1. declare variable USD set to 35.4
2. input value in NIO
3. multiply USD value by NIO
4. print result given
```
### 3.Answer to the question: Why is pseudocode helpful?
because it helps with the abstraction of the process that the code can follow and then it can be translated into any language
### 4.Create a pseudocode to calculate the aproximated age of a user base on the year they born, (you can define a variable with the actual year if you need it, like for example i could define Y <-- 2022)
```
1. define currentY as 2022
2. input year user was born as bornY
3. substract currentY - bornY as result
4. print result
```
### 5.Answer to the question: Why are flowcharts important to us as developers?
They are a useful way to explain your code to other programmers and what you pretend it to do. Also it works as the first step to define how you want the process to go because it can give you some perspective and help you travel through the code easily.
### 6. Search about High-level languages and Low-level languages, you can start with this video
* a high level language is user oriented, so it makes easier to convert and algorithm to code 
* a low level language is machine-oriented, so you need to be more specific in therms of capabilities and specifications, they are also known as assembly language

## Week challenges (Wednesday) 💻

### 1. Learn about binary, decimal and hexadecimal numbers
### 2. Translate the year you where born to binary, decimal and hexadecimal
The year I was born  can be translated as:
* decimal: 1998
* binary: 11111001110
* hexadecimal: 7CE
### 3. Translate 51966 into hexadecimal and binary
* binary: 1100101011111110
*  hexadecimal: CAFE > hahaha, really loved the easter egg
### 4. Use a Low-level language, for example MIPS aseembler, to do so, you will need to follow [this](resources/MIPS.md) guide. We recomend to check the guide first but also [this](https://courses.cs.vt.edu/cs2506/Fall2014/Notes/L04.MIPSAssemblyOverview.pdf) presentation could be helpful.
### 5. Base on the examples and the guide of the low-level language:
   5.1 Create a program to add two numbers given by the user
```
```
   5.2 Create a program that display your name
``` 
# create string
.data
str:  .asciiz "\nMy name is Walter G!\n"

.text
.globl main

main:
la $a0, str
li $v0, 4

# end the program
syscall
li $v0, 0
jr $ra
```
