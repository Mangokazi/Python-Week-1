# Python-Week-1
Day 1: INTRODUCTION AND ONBOARDING <br>
-We were taught how to install Python and Jupyter Notebook.<br>
-After installing the two we learnt about the use of neccessary prompts and ran a code on Jupyter.<br>
-I have also learnt that Jupyter is Python IDE(Integrated Development Environment).<br>
-Python may be used with any code editors, however, I will be using Jupyter Notebook.<br>
-There is a command that is used to access stored files which is, cd command. It is used to change directory.<br>
<br>
INTRODUCTION TO PYTHON:
 *Integers:
  -In this section I was struggling to understand an exercise on binary system and hexadecimal strings.
    Here is an example of the first problem I struggled with how my understand now:
     int('100', 2)
     Answer=4
     -Here I struggled to understand where the four was coming from, however now I do understand that in the binanry system, each digit 
      represents a power of 2. The first digit represents 2^0 which is 1, the next digit in the middle represents 2^1 which is 2, and the 
      last digit represents 2^2 which is 4.

      So the binary number 100 can be interpreted as follows:
       * 1 the first digit represents 2^2, which equals to 4
       * 0 in the middle represents 2^1, which equals to 0.
       * 0 in the last digit represents 2^0, which equals to 1.
         **Adding these up gives us: 4 + 0 + 0 = 4 , meaning 100 is equilavent to 4.
 -Second exercixe I struggled with under integers was this one:
    int('1ab', 16)
    *1ab is a hexadecimal string
    *16 is th base of specified for hexadecimal representation.

    *1 represents the value 1 in hex.
    *a represents the value 10 in hex.
    *b represents the value 11 in hex.
    *if we had another letter which was c, it would have hasd the value of 12.

    -Operators
     -Learnt the use of operators which is to manipulate and perform actions on data. Did an exercise using arithmetic operators as well as operators with strings.

*Data Structures
 -Did an intro to structures exercise.
 - Learnt about lists which may contain any data type, including a list within a list.
 - Lists may be useful when you need to  store large amount of data more efficienctly in memory.
 - Learnt what a dictionary, defined as a collection of key-value pairs. Dictionaries are declared using curly braces and accessed using keys.
   **Lists:
    -myList = [1,2,3,4,5]
     myList = [3:] - Start from index 3 but the end is not specified so it displays all variables from index to the end.
     myList = [0:6:2]- Start from from 0 to 6(exclusive). Using steps of 2.
     myList[::2] - Steps by 2. The start is not specified as well as the end, so it will display all variables from start to end.

   - for i in range(100): - Creates a sequence of numbers from 0 to 99(inclusive). So zero is also included( at index 0), which makes up to 100 numbers.
   
*Control Flow
 **Conditional Statements:
 -If/Else statement
   - Allows you to execute a block of code conditionally based on whether a certain condition is true or false
     **It has the synatax:
         a=3
         b=200
          if b > a:
            print("b is greater than a")
     -If statement can also be extended to with elif and else.

-For Loops
  -Used when the number of iterations is known in advance.
  -It consists of an initialization statement, a condition and an iteration statement. The loop executes as long as the statement is true.

-While Loops
 -Condition is evaluated before each iteration of the loop. If thew statement is true, the loop body is executed. If false the loop will terminate.

Pass
 -It is a null operation, nothing happens when it is executed.
 -It is used as a placeholder where some code is required but no action needs to be taken.

 Continue
  -Skips over certain lines within a loop, use the continue statement. Which will skip over any line that comes after it and jump back to the top of the loop to start the next iteration.

Break
 -I f you want to exit the early, use the break statement which will exit the loop and move on to the next line of code.
