<details>
  
<summary>Python-Week-1</summary>
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
 *Did an intro to structures exercise.
 * Learnt about lists which may contain any data type, including a list within a list.
 * Lists may be useful when you need to  store large amount of data more efficienctly in memory.
 * Learnt what a dictionary, defined as a collection of key-value pairs. Dictionaries are declared using curly braces and accessed using keys.
   **Lists:
    -myList = [1,2,3,4,5]
     myList = [3:] - Start from index 3 but the end is not specified so it displays all variables from index to the end.
     myList = [0:6:2]- Start from from 0 to 6(exclusive). Using steps of 2.
     myList[::2] - Steps by 2. The start is not specified as well as the end, so it will display all variables from start to end.

   - for i in range(100): - Creates a sequence of numbers from 0 to 99(inclusive). So zero is also included( at index 0), which makes up to 100 numbers.
   
*Control Flow
 **Conditional Statements:
 *If/Else statement
   * Allows you to execute a block of code conditionally based on whether a certain condition is true or false
     **It has the synatax:
         a=3
         b=200
          if b > a:
            print("b is greater than a")
     *If statement can also be extended to with elif and else.

*For Loops
  *Used when the number of iterations is known in advance.
  *It consists of an initialization statement, a condition and an iteration statement. The loop executes as long as the statement is true.

*While Loops
 *Condition is evaluated before each iteration of the loop. If thew statement is true, the loop body is executed. If false the loop will terminate.

Pass
 *It is a null operation, nothing happens when it is executed.
 *It is used as a placeholder where some code is required but no action needs to be taken.

 Continue
  *Skips over certain lines within a loop, use the continue statement. Which will skip over any line that comes after it and jump back to the top of the loop to start the next iteration.

Break
 *I f you want to exit the early, use the break statement which will exit the loop and move on to the next line of code.

Functions
 *A function is defined using the keyword def ( define) 
   def my_function():
    print("Hello from a function")

  my_function()
</details>
<details>
<summary>Python-Week-2</summary><br><br>
A function is  block of code that performs a specific task when the function is called. Functions are used to make code reusable, better organized, and more readable. They are composed of a name and parameters, which are denoted by the def statement: def MyFunction(num1, num2)<br>
Funcitions can have parameters and return values.<br>
There are FOUR basic types of functions in Python:
  -built-in function whichs which are an important part of Python.
  -functions that come from pre-installed modules.
  -user-defined functions which are written by users.
  -the lambda functions.<br><br>
  
-When you invoke a function, Python remembers the place where it happened and jumps into the invoked function.
-The body of the function is then executed.
-Reaching at the end of the function forces Python to return to the place directly after the point of invocation.<br>
-When you try to invoke a function before you define it, the NameError exception is thrown.<br>
 Example: hi()
          def hi():
           print("hi!")<br><br>
  Basic Function syntax:
   def  message():
     print("Enter next values:")
   print("We start here.")
   message()
   print("The end is here.")
   <br>
   Parameters and Arguments:<br>
   
   Parameters- Valriable defined within the parantheses during a function definition. They are written when declaring a function.
     Example: def sum(a, b) #parameters
                 print(a + b)
              sum(1, 2)
   <br>
   Argument- Value that is passed to a function when it is called. It might be a variable, value or object passed to a function or method as input.
   Example: def sum(a, b) 
                 print(a + b)
              sum(1, 2) #arguments
  <br>
  Types of arguments in python:
   - Positional arguments
   - Keyword arguments
     <br>
    Positional arguments:
      -Needed to be included in a proper order, the first argument is always listed first when the function is called, second argument needs to be called second and so on.
     <br>
     Keyword arguments:
      -It is an argument passed to a function or method which is preceded by a keyword and an equal sign. The order of the keyword with respect to another keyword does not matter because values are being explicitly assigned.
      -In order to handle keyword arguments, a method called kwargs can be used.
      -Keyword arguments have keys and values and can be passed in any order, so a dictionary is a more appropriate data strucutre for referencing them.

     Variables and Scope
      Function Scope:
       locals()-A function that allows access to all variables within a function without any asterisks. It is called locals because the variable it uses are only accessible locally within a function.<br>
       Docstring-The first string after the function is called the Document string or docstring. Ii is used to describe the functionality of the function. The use of a docstring optional but it is considered agood practice.
         Syntax:
           print(function_name._doc_)
  <br>
  Function within a function
  -Afunction thst is defined inside another function is known as the inner function or nested fuction. Nested functions can access variables of the enclosing scope. Inner functions are used so thst they can be protected from ecerything happening outside the function.
    Syntax: def f1():
              s='I love GeeksforGeeks'
             def f2():
               print(s)
             f2()
            f1()

Handling Errors and Exceptions
 -Errors in Python can be of two types i.e Syntax and Exceptions. Errors are problems in a program due to which program will stop the execution. Wjile exceptions are raised when some internal events occur which change the normal flow of the program.  <br>
 There are different types of exceptions:
  -SyntaxError
  -TypeError
  -NameError
  -IndexError
  -ValueError
  -KeyError
  -AttributeError
  -IOError
  ZeroDivisionError
  -ImportError
  <br>

  Difference between syntax error and exceptions
   -Syntax error- This error is caused by the wrong syntax in the code. It leads to termination of the program.<br>
   -Exceptions: Theyare raised when the program is syntactically correct, but the code results in an error. This error does not stop the execution of the program, however, it changes the normal flow of the program.<br>

   Try and Except Statements- Catching Exceptions
    -These two statements are used to catch and handle exceptions in Python. Statements that can raise exceptions are kept inside the try clause and the statements that are written inside except clause.
    -Use Case: Include a title, an actor (a user or system), and a scenario that describes how a goal is achieved. The scenario can be written as a paragraph or a list of steps in simple language. 
      
</details>
<details>
<summary>Python-Week-3</summary><br><br>

  On this week we learnt about the importance of project planning as were preparing to build and present our projects. This includes a GUI which is a graphical user interface for our projects.The project planning, the inspiration of the project as well as the aim.
![image](https://github.com/Mangokazi/Python-Week-1/assets/162969644/61e57cb5-97b4-4a1a-8ed1-286c7f3f02a9)
<br>
Stub code: Stub code is a piece of program used in software development to1234:
Stand in for some other programming functionality.
Simulate the behavior of existing code (such as a procedure on a remote machine).
Be a temporary substitute for yet-to-be-developed code.
Translate parameters sent between the client and server during a remote procedure call in distributed computing.
Convert parameters during a remote procedure call (RPC).
Be used as "placeholders" for specific applications that haven't been built yet.
  
</details>
