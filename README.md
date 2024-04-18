 
<details>
<summary>Python-Week-1</summary><br>
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
Be used as "placeholders" for specific applications that haven't been built yet.<br>

GUI Design planning: Planning a GUI design involves several steps:
Define the purpose: Understand what the application is supposed to do and what problems it will solve.
Understand the users: Know who will use the application and what their needs are.
Sketch out ideas: Create rough sketches of the GUI to explore different designs.
Create wireframes: Develop wireframes to establish the layout and elements of the interface.
Choose a color scheme and typography: Select colors and fonts that align with the brand and improve readability.
Develop prototypes: Build interactive prototypes to test functionality and user experience.
User testing: Conduct user testing to gather feedback and make necessary adjustments.
</details>
<details>
<summary>Data Analytics-Week-1&2</summary><br>
  

## Module 1: The Basics of Data
### Chapter 1: The Data Analyst
* What is data analytics?
  -Data analytics is the process of examining large sets of data to uncover patterns, trends, correlations, and insights that can be used to make informed decisions. It involves various techniques and tools to analyze data, including statistical analysis, machine learning algorithms, and data mining. It improves efficiency, effectiveness and profitability of work.
* The role of Data Analysts:
 -It is to transform raw data into actionable insights that guide decision-making processes within an organization. This involves several key responsibilities and skills.
  1. Data Collection:
     -Sourcing data from various channels, including databases, spreasdsheets, and external sources.
     -Cleaning and organising rthe data to ensure it is accurate, consistent, ready for analysis.
  2. Data analysis:
     -Employing statistical methods, machine learning techiques, or other analytical tools to interpret data.
     -Identifying trends, patterns, correlations that might notbe immediately obvious.
  3. Data visualization and storytelling:
     -Creating visual representations of the data, such as charts, graphs, and dashboards, to make complex information easily understandable,
     -Articulating findings in a compelling narrative to communicate the significance of the data to stakeholders.
  4. Decision Support:
     -Making recommendations based on data-driven insights to help guide business decisions,
     -Providing context around the data, including potential implications and future trends.
  5. Collaboration and Communication:
     -Working closely with other departments, such as marketing, finance, and operations, to understand their data needs and provide insights,
     -Effectively communicating complex data findings in a clear and concise manner to non-technical stakeholders,
  6. Continuous Learning and Adaptation:
     -Keeping up-to-date with the latest industry trends, tools, and technologies in data analysis.
     -Adapting to new types of data and analytical methods as the organization's needs evolve.
  * The analytics process:
     Data acquisition>> cleaning & manipulation>> analysis>> visualization>> reporting & communication
  * Analytics Techniques :
    - Descriptive Analytics
    - Predictive Analytics
    - Prescriptive Analytics
  *Role of Data Governance:Ensures the quality, security, and privacy of data throughout it's lifecycle.<br>
  ### Chapter 2: Understanding data
   * Data Types:  A data element is an attribute about a person, place, or thing containing data within a range of values. Data elements also describe characteristics of activities, including orders, transactions, and events.
   -  A data type limits the values a data element can have.
   *Tabular Data: abular data is data organized into a table, made up of columns and rows.
* Structured Data Structures:Structured data is tabular in nature and organized into rows and columns. Structured data is what typically comes to mind when looking at a spreadsheet. With clearly defined column headings, spreadsheets are easy to work with and understand. In a spreadsheet, cells are where columns and rows intersect.
  ![image](https://github.com/Mangokazi/Python-Week-1/assets/162969644/f7b9e1ec-645e-4b19-99d7-62abed108a14)
*Different data types:
-Numeric data
-Categorical data
-Text data
-Temporal data
-Spatial data
*Character Sets:
-Numeric
-Whole numbers
-Rational numbers
-Date and time
-Currently
*Unstructured data sets:
-Binary
-Audio
-Images
-Video
-Large text
*Structed Data
*Unstructured Data<br>
## Module 2: Data Preparation and Exploration
### Chapter 3: Databases and Data Acquisition
*Relational database:
-Relational databases store data in structured tables with rows and columns, where each row represents a record and each column represents a specific attribute or field.
Data in relational databases follows a predefined schema, which defines the structure, data types, and relationships between tables.
Relational databases use SQL (Structured Query Language) for querying and managing data.
Examples of relational database management systems (RDBMS) include MySQL, PostgreSQL, Oracle Database, Microsoft SQL Server, and SQLite.
Relational databases are well-suited for applications that require ACID (Atomicity, Consistency, Isolation, Durability) transactions, complex queries, and strong data consistency guarantees.

*Nonrelational databases:
-Nonrelational databases, also known as NoSQL databases, are designed to handle large volumes of unstructured or semi-structured data and provide flexible data models.
Unlike relational databases, NoSQL databases do not strictly adhere to a predefined schema, allowing for dynamic schema evolution and schema-less data storage.
NoSQL databases support various data models, including document-oriented, key-value, column-family, and graph databases, catering to different types of data and use cases.
Examples of NoSQL databases include MongoDB (document-oriented), Apache Cassandra (column-family), Redis (key-value), Neo4j (graph), and Amazon DynamoDB (document-oriented and key-value).
NoSQL databases are often chosen for applications that require scalability, high availability, and flexible data models, such as web applications, real-time analytics, and content management systems.
*Entity-Relationship Diagram:
-An Entity-Relationship Diagram (ERD) is a visual representation of the entities and relationships within a database. It's a powerful tool for database design as it helps to visualize the structure of the database and understand how different entities are related to each other.

In an ERD, entities are represented by rectangles, and relationships between entities are represented by lines connecting them. Each entity has attributes, which are the properties or characteristics of the entity. Attributes are typically listed within the entity rectangle.
Entities: Entities represent the real-world objects or concepts that are modeled in the database. For example, in a university database, entities might include Student, Course, and Instructor.

Relationships: Relationships represent how entities are connected or related to each other. There are different types of relationships, such as one-to-one, one-to-many, and many-to-many. For example, a Student entity might have a relationship with a Course entity indicating that a student can enroll in multiple courses.

Attributes: Attributes represent the properties or characteristics of entities. Each entity has its own set of attributes. For example, attributes of a Student entity might include StudentID, Name, and DateOfBirth.<br>
         ![image](https://github.com/Mangokazi/Python-Week-1/assets/162969644/02010eea-7bfe-447a-889d-5daeb3a1119a)
*Cardinality:
-Cardinality refers to the relationship between two entities, showing how many instances of one entity relate to instances in another entity. You specify cardinality in an ERD with various line endings. The first component of the terminator indicates whether the relationship between two entities is optional or required. The second component indicates whether an entity instance in the first table is associated with a single entity instance in the related table or if an association can exist with multiple entity instances. <br>
         ![image](https://github.com/Mangokazi/Python-Week-1/assets/162969644/21f79a92-0d63-45e9-8485-83c82e5afef3)
*Data Manipulation
-When manipulating data, one of four possible actions occurs:
-Create new data.
-Read existing data.
-Update existing data.
-Delete existing data.<br>

Reading and manipulating data is commonplace on the path to creating insights. To that end, we will focus on options that affect reading data. Before jumping in, it is helpful to understand the syntax of a query.
![image](https://github.com/Mangokazi/Python-Week-1/assets/162969644/fd909233-2461-45d0-8d9f-66c8169cbddb)
*Select:
-The SELECT clause is used to retrieve data from a database. It is one of the fundamental clauses in SQL queries. 
Example:
SELECT column1, column2, ...
FROM table_name;
 <br>
 *From:
 -The FROM clause in a query identifies the source of data, which is frequently a database table. Both the SELECT and FROM clauses are required for a SQL statement to return data, as follows:
<br>
*Filtering:
-Filtering in SQL is done using the WHERE clause within the SELECT statement. The WHERE clause allows you to specify conditions that the rows must meet in order to be included in the result set. 
Example:
SELECT column1, column2, ...
FROM table_name
WHERE condition;
<br>
*Sorting:
-Sorting in SQL is done using the ORDER BY clause within the SELECT statement. The ORDER BY clause allows you to specify the order in which the result set should be sorted based on one or more columns.
Example:
SELECT column1, column2, ...
FROM table_name
ORDER BY column_name [ASC | DESC];
<br>
*Date funtions:
-SQL provides various date functions to manipulate and work with date and time data. Some commonly used date functions include:
*Current date: SELECT CURRENT_DATE;
*Current time: SELECT CURRENT_TIME;
*CURRENT_TIMESTAMP: SELECT CURRENT_TIMESTAMP;
*DATE_FORMAT: SELECT DATE_FORMAT(date_column, 'format_string') FROM table_name;
*DATE_ADD: SELECT DATE_ADD(date_column, INTERVAL 1 DAY) FROM table_name;
*DATE_SUB: SELECT DATE_SUB(date_column, INTERVAL 1 MONTH) FROM table_name;
*DATEDIFF: SELECT DATEDIFF(end_date, start_date) FROM table_name;
*DATE: SELECT DATE(datetime_column) FROM table_name;
*EXTRACT: SELECT EXTRACT(YEAR FROM date_column) FROM table_name;
<br>
*Logical Functions:







</details>
