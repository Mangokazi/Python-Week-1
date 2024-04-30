 
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
![image](https://github.com/Mangokazi/Python-Week-1/assets/162969644/fd909233-2461-45d0-8d9f-66c8169cbddb)<br>
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
### Chapter 4: Data Quality
* Data quality refers to the reliability, accuracy, consistency, completeness and relevance of data. It is about having data that is ft for it's intended purpose.
* Accuracy
* Completeness
* Consistency
* Relevance<br>
-The purpose of data quality is to improve decision making.
- Challenges within data quality:
* Errors
* Duplicates
* Incomplete data
* Outdated data
-Tool:
*Data cleaning softwares
* KPIs
<br>
- Duplicate data:
* Duplicate data occurs when data representing the same transaction is accidentally duplicated within a system. Suppose you want to open a spreadsheet on your local computer. To open the spreadsheet, you locate the file and double-click it. This method of opening documents establishes muscle memory that associates double-clicking with the desired action.<br>
![image](https://github.com/Mangokazi/Python-Week-1/assets/162969644/1dca59a2-46bc-425a-99a2-0b148c4c20f0)<br>
-Redundant data:
* While duplicate data typically comes from accidental data entry, redundant data happens when the same data elements exist in multiple places within a system. Frequently, data redundancy is a function of integrating multiple systems.<br>
![image](https://github.com/Mangokazi/Python-Week-1/assets/162969644/9f4f5a12-0d5e-4d35-a418-da9d701a8064)<br>

-Data Blending:
*Data blending combines multiple sources of data into a single dataset at the reporting layer. While data blending is conceptually similar to the extract, transform, and load process in Chapter 3, there is a crucial difference. Recall that ETL processes operate on a schedule, copying data from source systems into analytics environments. Business requirements drive the scheduling, such as near real-time, hourly, daily, weekly, monthly, or annually. Typically, an organization's IT department designs, builds, operates, and maintains ETL processes.<br>
### Chapter 5: Data Analysis and Stastics
* Fundamentals of Statistics:
* _One key concept is the definition of a population. A population represents all the data subjects you want to analyze. For example, suppose you are an analyst at the National Highway Traffic Safety Administration (NHTSA) and start to receive reports about a potential defect in Ford F-Series trucks. In this case, the population is all Ford F-Series trucks. If you want to examine all Ford F-Series vehicles, you'd have to conduct a census. A census is when you obtain data for every element of your population. Conducting a census is typically infeasible due to the effort involved and the scarcity of resources.
* Descriptive Statistics:
* -Descriptive statistics is a branch of statistics that summarizes and describes data. As you explore a new dataset for the first time, you want to develop an initial understanding of the size and shape of the data. You use descriptive statistics as measures to help you understand the characteristics of your dataset.

When initially exploring a dataset, you may perform univariate analysis to answer questions about a variable's values. You also use descriptive measures to develop summary information about all of a variable's observations. This context helps orient you and informs the analytical techniques you use to continue your analysis.
*Measures of Frequency:
-Measures of frequency help you understand how often something happens. When encountering a dataset for the first time, you want to determine how much data you are working with to help guide your analysis. For example, suppose you are working with human performance data. One of the first things to understand is the size of the dataset. One way to accomplish this quickly is to count the number of observations.
*Measures of Central Tendency:
-To help establish an overall perspective on a given dataset, an analyst explores various measures of central tendency. You use measures of central tendency to identify the central, or most typical, value in a dataset. There are numerous ways to measure central tendency, and you end up using them in conjunction with each other to understand the shape of your data.
*Confidence Intervals:
-Each time you take a sample from a population, the statistics you generate are unique to the sample. In order to make inferences about the population as a whole, you need a way to come up with a range of scores that you can use to describe the population as a whole. A confidence interval describes the possibility that a sample statistic contains the true population parameter in a range of values around the mean. When calculating a confidence interval, you end up with a lower bound value and an upper bound value. Given the confidence interval range, the lower bound is the lower limit, and the upper bound is the upper limit.
*Simple Linear Regression:
-Simple linear regression is an analysis technique that explores the relationship between an independent variable and a dependent variable. You can use linear regression to identify whether the independent variable is a good predictor of the dependent variable. You can perform a regression analysis in spreadsheets like Microsoft Excel and programming languages, including Python and R. When plotting the results of a regression, the independent variable is on the x-axis and the dependent variable is on the y-axis.
### Chapter 6: Data Analytics Tools
*Structured Query Language (SQL):
-The Structured Query Language (SQL) is the language of databases. Any time a developer, administrator, or end user interacts with a database, that interaction happens through the use of a SQL command. SQL is divided into two major sublanguages:

The Data Definition Language (DDL) is used mainly by developers and administrators. It's used to define the structure of the database itself. It doesn't work with the data inside a database, but it sets the ground rules for the database to function.
The Data Manipulation Language (DML) is the subset of SQL commands that are used to work with the data inside of a database. They do not change the database structure, but they add, remove, and change the data inside a database.
*Machine Learning:
-Moving on from statistics-focused tools, the industry also makes use of a set of graphical tools designed to help analysts build machine learning models without requiring them to actually write the code to do so. These machine-learning tools aim to make machine-learning techniques more accessible. Analysts may still tune the parameters of their models but do not necessarily need to write scripts to do so.
*Analytics Suites
-programming languages that allow skilled developers to complete whatever analytic task face them and specialized tools, such as spreadsheets, statistics packages, and
machine learning tools that focus on one particular component of the analytics process.
*Microsoft Power BI
-Power BI is Microsoft's analytics suite built on the company's popular SQL Server database platform. Power BI is popular among organizations that make widespread use of other Microsoft software because of its easy integration with those packages and cost-effective bundling within an organization's Microsoft enterprise license agreement.

The major components of Power BI include the following:

Power BI Desktop is a Windows application for data analysts, allowing them to interact with data and publish reports for others.
The Power BI service is Microsoft's software-as-a-service (SaaS) offering that hosts Power BI capabilities in the cloud for customers to access.
Mobile apps for Power BI provide users of iOS, Android, and Windows devices with access to Power BI capabilities.
Power BI Report Builder allows developers to create paginated reports that are designed for printing, email, and other distribution methods.
Power BI Report Server offers organizations the ability to host their own Power BI environment on internal servers for stakeholders to access.
*MicroStrategy
MicroStrategy is an analytics suite that is less well-known than similar tools from IBM and Microsoft, but it does have a well-established user base. MicroStrategy offers many of the same tools as its counterparts, making it easy for users to build dashboards and reports and apply machine learning techniques to their business data.
</details>
<details>
<summary>Data Governance</summary><br>
 
# Data Governance: Chapter 1
### What is data?
- Data refers to facts, figures, or information, often in the form of numbers, text, or multimedia, that are collected, stored, and analyzed for various purposes. It can be anything from simple measurements to complex multimedia files, and it can represent almost anything, from business transactions to scientific observations to personal preferences.
### Data can be classified into two main types:
- Structured Data: This type of data is highly organized and formatted in a way that makes it easily searchable and analyzable. Structured data often resides in databases and is represented in tables with rows and columns. Examples include spreadsheets, SQL databases, and CSV files.<br>
- Unstructured Data: This type of data lacks a specific structure and is not easily organized in a traditional database format. Unstructured data includes text documents, images, videos, social media posts, emails, and more. Analyzing unstructured data often requires advanced techniques such as natural language processing (NLP) or computer vision.<br>
- Data is an important important resource an oganization possesses in today's economy.
- Despite the fact that all organizations handle and control data, a significant number struggle to do so effectively. This leads to missed opportunities for business growth, revenue enhancement, and the utilization of crucial insights. Moreover, these organizations expose themselves to increased risk in a world fraught with complicated regulatory demands and devastating cyberattacks.
### What is data governance?
- Data governance is a framework that defines the rules, policies, procedures, and responsibilities for managing and ensuring the quality, availability, integrity, and security of an organization's data throughout its lifecycle. It provides a structured approach to managing data assets and helps organizations ensure that their data is used effectively, responsibly, and in compliance with regulatory requirements.
### Key components of data governance include:
- Data Quality Management: Ensuring that data is accurate, complete, consistent, and relevant for its intended purpose.
- Data Stewardship: Assigning responsibility for managing specific data assets to individuals or teams within the organization, known as data stewards.
- Data Security and Privacy: Establishing measures to protect data from unauthorized access, loss, or corruption, and ensuring compliance with relevant privacy regulations such as GDPR (General Data Protection Regulation) or CCPA (California Consumer Privacy Act).
- Data Lifecycle Management: Defining processes for the creation, storage, usage, archival, and disposal of data to ensure it remains relevant and valuable over time.
- Data Standards and Policies: Establishing guidelines, standards, and best practices for data management, including naming conventions, data classification, and data retention policies.
- Data Access and Authorization: Controlling who has access to what data and under what circumstances, ensuring that access is granted based on roles and responsibilities.
- Data Compliance and Risk Management: Ensuring that data practices comply with relevant laws, regulations, and industry standards, and mitigating risks associated with data management.
- Data Governance Council or Committee: Establishing a governing body responsible for setting data governance strategy, policies, and priorities, often composed of senior executives and representatives from different departments.
  ### Data Governance VS Data Management
- Data governance and data management are related concepts that work together to ensure the effective use and management of data within an organization, but they focus on different aspects of the data lifecycle.
 ### Data Governance:
 
Focus:<br>
- Data governance focuses on the overall strategy, policies, and framework for managing and ensuring the quality, availability, integrity, and security of data.<br>
Purpose:<br>
- The primary purpose of data governance is to establish rules, guidelines, and processes to ensure that data is used effectively, responsibly, and in compliance with regulatory requirements.<br>
Components:<br>
- Data governance involves defining the roles and responsibilities of stakeholders, establishing policies and standards, managing data quality, ensuring compliance, and enforcing data security and privacy measures.
Example: A data governance program might involve creating a data governance council, developing data policies and standards, assigning data stewards, and monitoring adherence to data governance principles.
### Data Management:

Focus:<br>
- Data management focuses on the practical aspects of handling data throughout its lifecycle, including collection, storage, processing, and analysis.<br>
Purpose:<br>
- The purpose of data management is to ensure that data is stored efficiently, organized effectively, and used appropriately to support the organization's goals and objectives.<br>
Components:<br>
- Data management involves activities such as data collection, data storage, data integration, data cleaning, data modeling, data analysis, and data archiving.
Example: Data management activities might include implementing a data warehouse for storing and organizing data, developing ETL (Extract, Transform, Load) processes to integrate data from multiple sources, and implementing data quality tools to clean and standardize data.
### Data Gorvanance VS Information Governance
-Data governance and information governance are closely related concepts, but they have slightly different scopes and focuses:
### Data Governance:
Focus:<br>
- Data governance primarily focuses on the management, quality, security, and usability of the organization's data assets.<br>

Scope:<br>
- Data governance deals specifically with the governance of data, which includes structured data (such as databases and spreadsheets) and unstructured data (such as documents, emails, and multimedia files).<br>

Purpose:<br>
- The purpose of data governance is to establish rules, processes, and standards to ensure that data is managed effectively, responsibly, and in compliance with regulatory requirements.<br>

Components:<br>
Data governance involves defining data ownership, roles, and responsibilities, establishing data policies and standards, managing data quality, ensuring data security and privacy, and enforcing compliance measures.
Example: Implementing data governance might involve creating a data governance council, developing data policies and standards, assigning data stewards, and implementing data quality tools.
### Information Governance:
Focus:<br> Information governance has a broader focus that extends beyond just data to include all types of information assets within the organization, including data, documents, records, and knowledge.<br>

Scope:<br>
- Information governance covers not only structured and unstructured data but also other types of information assets, such as documents, records, and intellectual property.<br>

Purpose:<br>
- The purpose of information governance is to manage and protect all information assets in a holistic manner, ensuring their integrity, availability, security, and compliance.<br>
Components:<br>
- Information governance encompasses data governance but also includes additional elements such as document management, records management, knowledge management, and compliance management.
Example: Implementing information governance might involve developing a comprehensive information governance framework that covers data governance, document management, records management, knowledge management, and compliance management.<br>
### The Value of Data Governance
- Data governance holds significant value for organizations across various industries due to several key benefits it provides:<br>
- Data Quality Improvement: Data governance ensures that data is accurate, consistent, complete, and reliable. By establishing data quality standards and processes, organizations can improve the quality of their data, leading to better decision-making and increased trust in data-driven insights.
- Compliance and Risk Management: Data governance helps organizations comply with regulatory requirements and mitigate risks associated with data management. By enforcing data security, privacy, and compliance measures, organizations can avoid penalties, legal issues, and reputational damage.
- Increased Trust and Confidence: With data governance in place, stakeholders have increased trust and confidence in the organization's data. This trust leads to greater reliance on data-driven decision-making, fostering a culture of data-driven insights across the organization.
- Enhanced Decision-Making: Quality data that is governed properly provides a solid foundation for decision-making at all levels of the organization. With accurate and timely data available, executives can make informed decisions quickly, leading to improved business outcomes and competitive advantage.
- Cost Reduction and Efficiency: Data governance helps eliminate data silos, redundancies, and inconsistencies, leading to cost savings and increased operational efficiency. By streamlining data management processes and optimizing data usage, organizations can reduce wastage and improve resource allocation.
- Improved Collaboration and Communication: Data governance encourages collaboration and communication among stakeholders across departments. By defining roles, responsibilities, and data standards, organizations can facilitate better coordination and alignment, leading to smoother workflows and improved outcomes.
- Data Asset Valuation: Well-governed data assets are more valuable to the organization. By ensuring data quality, security, and compliance, organizations can maximize the value of their data assets, leading to better financial performance and market competitiveness.
- Support for Data-Driven Innovation: Data governance provides a solid foundation for data-driven innovation initiatives. With properly governed data, organizations can explore new opportunities, develop innovative products and services, and adapt to changing market conditions more effectively.
- Customer Satisfaction and Loyalty: By ensuring data accuracy and privacy, organizations can enhance customer satisfaction and loyalty. Customers are more likely to trust organizations that handle their data responsibly, leading to stronger relationships and increased customer retention.
### The most common elements of a data governance program.
![image](https://github.com/Mangokazi/Python-Week-1/assets/162969644/3f785a99-e2ce-4963-b842-19adf47984d0)<br>

###  Common components of a data governance framework.
![image](https://github.com/Mangokazi/Python-Week-1/assets/162969644/132ebc1b-1a15-43dc-ab18-540d62e309d7)<br>

###  What is data culture?
-Data culture refers to the attitudes, behaviors, and practices within an organization that prioritize the collection, analysis, and use of data to drive decision-making and achieve organizational goals. It's about fostering an environment where data is valued, trusted, and utilized effectively at all levels of the organization.<br>
### Key components of a data culture include:
- Data Literacy: Employees across the organization have the necessary skills and knowledge to understand, interpret, and analyze data. This includes basic data literacy as well as more advanced skills in data analysis, statistics, and data visualization.
- Data-Driven Decision Making: Decision-making processes are guided by data and evidence rather than intuition or gut feelings. Leaders and employees use data to inform their decisions, identify opportunities, and solve problems.
- Openness and Transparency: Data is shared openly across the organization, and there is transparency about how data is collected, analyzed, and used. This fosters trust in data and encourages collaboration and knowledge sharing.
- Continuous Learning and Improvement: The organization promotes a culture of continuous learning and improvement based on data insights. Feedback loops are established to monitor outcomes, learn from successes and failures, and adapt strategies accordingly.
- Empowerment and Accountability: Employees are empowered to access and analyze data relevant to their roles and responsibilities. They are accountable for the quality of data they produce and the decisions they make based on that data.
- Data-Driven Goals and KPIs: Goals and Key Performance Indicators (KPIs) are defined and measured using data to track progress and performance. This ensures alignment with organizational objectives and enables data-driven evaluation of success.
- Data Governance and Security: The organization has established data governance policies and practices to ensure data quality, security, and compliance with regulations. Data privacy and security are prioritized to protect sensitive information.
- Leadership Support and Advocacy: Leadership plays a crucial role in fostering a data culture by setting the tone, providing resources, and championing data initiatives. Leaders demonstrate the value of data-driven decision-making through their actions and behaviors.
- Innovation and Experimentation: Data is used to drive innovation and experimentation within the organization. Employees are encouraged to explore new ideas, test hypotheses, and learn from data-driven experiments.
- Integration of Data into Workflows: Data is integrated into everyday workflows and processes, making it easily accessible and actionable for employees. This includes using data tools and technologies to automate data processes and provide real-time insights.
- ### Assessing data culture
- Leadership Commitment and Support:
Are senior leaders actively promoting the use of data for decision-making?
Do leaders allocate resources and invest in data initiatives?
Are data-driven behaviors demonstrated by leaders?
- Data Literacy and Skills:
What is the level of data literacy across different departments and roles?
Are employees equipped with the necessary skills to work with data effectively?
Are training programs or resources available to improve data literacy?
- Data Accessibility and Infrastructure:
Is data easily accessible to employees who need it?
Are there centralized data repositories or platforms for accessing and analyzing data?
How reliable and up-to-date is the data infrastructure?
- Data Quality and Trust:
Is there confidence in the accuracy and reliability of the data?
Are there processes in place to monitor and improve data quality?
Do employees trust the data they use for decision-making?
- Data-Driven Decision Making:
Are decisions informed by data and evidence?
Is there a clear process for using data to guide decision-making?
Do employees have access to the data needed to support decision-making?
- Collaboration and Communication:
Is there a culture of sharing data and insights across teams and departments?
Are there regular meetings or forums for discussing data and insights?
Do employees collaborate on data-driven projects or initiatives?
- Experimentation and Innovation:
Are employees encouraged to experiment and explore new ideas using data?
Are there processes in place for testing hypotheses and learning from data-driven experiments?
Is there a willingness to take calculated risks based on data insights?
- Feedback and Learning:
Is feedback collected on data initiatives and processes?
Are there mechanisms for learning from successes and failures?
Is there a culture of continuous improvement based on data insights?
- Data Governance and Compliance:
Are there established data governance policies and practices?
Is data governance integrated into everyday workflows and processes?
Are data privacy and security measures in place to protect sensitive information?
Employee Engagement and Recognition:
Are employees engaged in data-related activities and initiatives?
Are achievements and contributions in data-driven projects recognized and rewarded?
Do employees feel valued for their data-related skills and efforts?
## Assessing Data Governance Readiness
- Assessing data governance readiness involves evaluating an organization's readiness to implement and sustain an effective data governance program.<br>

The following basic checklist of items will help you determine the data governance readiness of your organization:<br>

- The basis of a data culture exists.
- The program is 100 percent aligned with business strategy.
- Senior leadership is 100 percent committed to the program and its goals.
- Senior leadership understands this is a strategic, enterprise program and not the sole responsibility of the IT department.
- One or more sponsors have been identified at an executive level.
- The program has the commitment to fund its creation and to maintain it in the long term.
- The organization understands this is an ongoing program and not a one-off project.
- You have documented the return-on-investment (ROI).
- Legal and compliance teams (internally or externally) understand and support the goals of the program.
- Fundamental data skills exist for the data governance journey.
- The IT organization is capable and resourced to support the program.
# Chapter 2: Exploring a World Overflowing with Data
### What is a zettabyte?
- A zettabyte is a unit of digital information storage equal to 1,000 exabytes, 1,000,000 petabytes, or 1,000,000,000 terabytes.

To give you a sense of scale:

- 1 zettabyte is equivalent to 1,000,000,000,000,000,000,000 bytes.
- It's often abbreviated as "ZB."
- In simpler terms, a zettabyte is an enormous amount of data storage capacity. It's far beyond what an average person can easily comprehend. To put it in context:

- A single zettabyte could hold billions of hours of HD video, millions of years' worth of music, or countless documents and images.
- The entire world's digital data produced in a year might reach into the zettabyte range.
- The exponential growth of data generated each year has made zettabytes more relevant. With the increasing use of the internet, social media, cloud computing, and the Internet of Things (IoT), it's expected that the global data volume will continue to grow rapidly, possibly reaching zettabyte levels sooner than we might imagine.
### The qualitative and quantitative nature of data types
![image](https://github.com/Mangokazi/Python-Week-1/assets/162969644/a7b4cfef-8134-45d3-9a22-478f02f9aaa0)<br>
### From Data to Insight
- Data refers to raw facts, figures, or symbols that represent information. It is often unprocessed and lacks context until it's organized or interpreted.

- Information, on the other hand, is processed, organized, and structured data that has context, meaning, and relevance for a specific purpose or audience.
### Illustrates the journey from data to insight
  ![image](https://github.com/Mangokazi/Python-Week-1/assets/162969644/9cc14922-4d52-4d85-a924-e109dc35af7c)<br>
### Data Ownership
-Data ownership describes the rights a person, team, or organization has over one or more data sets. These rights may span from lightweight oversight and control to rigorous rules that are legally enforceable. For example, data associated with intellectual property — items such as copyrights and trade secrets — will likely have high degrees of protection, from accessibility rights to who can use the data and for what purpose.
### Data Architecture
- Data architecture refers to the design and structure of an organization's data assets, including how data is collected, stored, processed, managed, and utilized. It provides a blueprint for managing data effectively to support business objectives and information needs.<br>
Here's a breakdown of key components of data architecture:<br>
- Data Sources and Collection:<br>
Identifies the various sources of data within and outside the organization, such as databases, applications, sensors, devices, and external data providers.
Defines mechanisms for collecting, extracting, and ingesting data from these sources into the data environment.
- Data Storage:<br>
Determines how data is stored and organized for efficient access and retrieval.
Includes considerations for storage technologies, such as relational databases, data warehouses, data lakes, NoSQL databases, and cloud storage.
Defines data structures, schemas, and models to organize and represent data.
- Data Processing and Transformation:<br>
Describes how data is processed, transformed, and prepared for analysis or consumption.
Involves data integration, ETL (Extract, Transform, Load) processes, data cleansing, data enrichment, and data aggregation.
Considers technologies like ETL tools, data pipelines, and data processing frameworks.
- Data Governance and Metadata:<br>
Establishes policies, standards, and processes for managing data quality, security, and compliance.
Defines metadata standards and practices for documenting data assets, including data lineage, data definitions, and data ownership.
Ensures adherence to regulatory requirements and industry standards.
- Data Access and Consumption:<br>
Specifies how users and applications access and consume data.
Includes data access methods, APIs, query languages, and data visualization tools.
Addresses security, authentication, and authorization requirements for controlling data access.
- Data Architecture Patterns:<br>
Defines common patterns and architectures for specific use cases or data processing requirements.
Examples include transactional systems, data warehouses, data lakes, real-time analytics, and event-driven architectures.
Determines the appropriate architectural components and technologies for each pattern.
- Scalability and Performance:<br>
Considers scalability requirements to handle increasing data volumes and user loads.
Addresses performance optimization techniques for efficient data processing and analysis.
Evaluates technologies and architectures that support horizontal and vertical scaling.
- Data Lifecycle Management:<br>
Defines processes and policies for managing data throughout its lifecycle, from creation to archival or deletion.
Includes data retention policies, data archival strategies, and data disposal procedures.
Ensures compliance with legal and regulatory requirements.







 
</details>
