name = input("Enter Name:").upper()
while True:
    print("=" * 140)
    print(f"""                                        WELCOME TO PYTHON TUTORIAL {name}
                                You will learn Python and participate in a fun and amazing Q&A.
                                        You will only have 3 lives in the Game.""")
    print("=" * 140)
    print("""1 - Prelim
2 - Midterm
3 - Finals
0 - Exit""")
    major = input("Choose between Prelim, Midterm, Finals or Exit: ").strip()
    print("=" * 140)
    if major == "1":
        print("""1 - INTRODUCTION TO PROGRAMMING
2 - PYTHON BASIC SYNTAX
3 - PRINTING OUTPUT
4 - PYTHON COMMENTS
5 - VARIABLES, CONSTANTS, AND DATA TYPES IN PYTHON
6 - BASIC DATA TYPES IN PYTHON
7 - ARITHMETIC OPERATORS AND EXPRESSIONS
8 - BASIC INPUT AND OUTPUT IN PYTHON
0 - EXIT""")
        lesson = input("CHOSE A LESSON (0-8): ").strip()
#Introducton to programming
        if lesson == "1":
            print("""===========================================================================================================================================                                     
                                            INTRODUCTION TO PROGRAMMING
                                      
===========================================================================================================================================                                      
PROGRAMMING LANGUAGE - is a special language that computers understand and use to perform tasks.
COMMON PROGRAMMING LANGUAGE INCLUDES: Python,C/C++,PHP,Java,Javascript,Ruby.
PYTHON - is a widely used programming language that was created by GUIDO VAN RUSSOM in 1991 and He was a DUTCH SOFTWARE ENGINEER.
PYTHON - is a HIGH-LEVEL, INTERPRETED, and GENERAL-PURPOSE PROGRAMMING LANGUAGE design to be simple,readable, and easy to learn.
WHY LEARN PYTHON?
1.SIMPLE and EASY TO LEARN - Great for beginners.
2.READABLE SYNTAX - Code looks almost like English.
3.VERSATILE - Used in many fields (AI,Web,Automation,Games,etc.)
4.HUGE COMMUNITY - Lots of support,tutorials and libraries.
WHAT DO YOU NEED TO START PYTHON PROGRAMMING?
PROFESSINALS IDES/ CODE EDITORS
PYCHARM (by jetbrains)   VS CODE (Visual Studio Code) JUPYTER NOTEBOOK / JUPYTERLAB.
==========================================================================================================================================""")
#Question for Introduction To Programming
            questions = [
                ("Q1: What Special Language is used that computers understand?\nA) Programming Language  B) Print()  C) English\nAnswer: ", "a"),
                ("Q2: Is Javarice a Common Programming Language?\nA) Yes  B) No  C) Maybe\nAnswer: ", "b"),
                ("Q3: Who Created the Python?\nA) RJ Russom  B) Van RJ Russom   C) Guido Van Russom\nAnswer: ", "c"),
                ("Q4: What Year was Python Created?\nA) 1991  B) 1981  C) 1999\nAnswer: ", "a"),
                ("Q5: Learn Python because its?\nA) Simple and Hard  B) Simple and Easy to Learn  C) Useful  \nAnswer: ", "b"),
                ("Q6: It is used in many fields.\nA) Readable Syntax  B) Language  C) Versatile\nAnswer: ", "c"),
                ("Q7: Does Huge Community have a lot of support, tutorials and libraries.?\nA) Yes  B) No   C) Maybe\nAnswer: ", "a"),
                ("Q8: What does Code almost look like?\nA) Math   B) English  C) Language\nAnswer: ", "b"),
                ("Q9: Python is design to be?\nA) Simple and Hard  B) Hard  C) Readable\nAnswer: ", "c"),
                ("Q10: Is Python Great for beginners?.\nA) Yes B) No  C) Maybe\nAnswer: ", "a"),
            ]
#Python Basic Syntax            
        elif lesson == "2":
            print("""===========================================================================================================================================                                     
                                           PYTHON BASIC SYNTAX
                                      
===========================================================================================================================================
What is PYTHON SYNTAX
SYNTAX - Refers to the set of rules that tells us how to correctly write a program in python.

PYTHON SYNTAX

1.PYTHON is CASE-SENSITIVE - python treats uppercase and lowercase letters differently.
*CORRECT 
1 name = "John" --- Create variable name
2 print(name)   --- Print the value of name
*INCORRECT 
1 name = "John" --- Error name is not as the same name
2 print(Name)   --- Python is case-sensetive
2.INDENTATION - unlike other programming languages, Python uses indentation (space) to define blocks of code.
*CORRECT
1 age = 18 --- assign value to Variable
2
3 if age >= 18: --- Check condition
4     print("Adult") --- Indented (inside the block) 
*INCORRECT
1  age = 18
2  
3  if age >= 18:
4  print("Adult") --- Not indented (outside the block)
==========================================================================================================================================""")
#Queston for Python Basic Syntax
            questions = [
                ("Q1: This refers to the set of rules that tells us how to correctly write a program in python.\n A) Syntax B) Rules C) Set\nAnswer: ", "a"),
                ("Q2: What do you call that treats uppercase and lowercase in pythons letter differently.\n A) Sensetive B) Case-sensetive C) Python\nAnswer: ", "b"),
                ("Q3: Unlike other programming languages, Python uses indentation to define blocks of code. What does indentation mean?\nA) Equal B) Minus C) Space \nAnswer: ", "c"),
                ("Q4: name =  ''John'', Which is correct to print John. \nA) print(name)   B) print(NAMe)    C) print(Name)\nAnswer: ", "a"),
                ("Q5: Python needs indentation to define blocks of the code. after age = 18 Where would you put the print(age).\nA) Next to age = 18 B) Lower to the age = 18 just like how we put the age that how we would put it C) Right above the age = 18\nAnswer: ", "b"),
            ]
#Printing output
        elif lesson == "3":
            print("""===========================================================================================================================================
                                        PRINTING OUTPUT
            
===========================================================================================================================================
PRINT STATEMENT
The print() function displays information on the screen.
SYNTAX:
print(value)

print - The function that display output.
() - parentheses that contain the information to be displayed.
value - The text,number,variable, or expression you want to show.
PRINTING TEXT
TEXT (also called a string) must be enclosed in QUOTATION MARKS.
* COREECT 
print("Hello World!") --- Correct syntax uses double quotes inside the parentheses.
*INCORRECT
print(hello,World!) Incorrect syntax Missing quotes around the text.
PRINTING NUMBERS
You can PRINT NUMBERS directly without quotation marks.
                  OUTPUT  Numbers (int,float) Numbers are used without quotes.
1 print(100)  --- 100      these are treated as numbers by Python.
2 print(25.5) --- 25.5    
ALSO CORRECT (DIFFERENT DATA TYPES)
                   OUTPUT   strings (str)
1 print("100")  --- 100     Value inside quotes are text (string). 
2 print("25.5") --- 25.5    output looks the same but they are treated as text (string) in python.
KEY DIFFERENCE
The output is the same, but the data type is different.
NUMBER (int/float)  STRING (str)           Remember: 
print(type(100))    print(type("100"))     Use quotes for text,not for numbers.
OUTPUT              OUTPUT
<class 'int'>       <class 'str'>
==========================================================================================================================================""")
#Question For Printing Output
            questions = [
                ("Q1: Prints function is to What?\nA) Displays Information on the Screen B) To Display Text Messages C) To Display Numbers\nAnswer: ", "a"),
                ("Q2: The function that displays output.\nA) Text B) Print C) Numbers\nAnswer: ", "b"),
                ("Q3: The that contains information to be displayed.\nA) Dot B) Space C) Parentheses\nAnswer: ", "c"),
                ("Q4: What do you call that holds Text,Number,variable or expression that you want to show.\nA) Value B) Numbers C) Text\nAnswer: ", "a"),
                ("Q5: Text is also called as?\nA) Numbers B) String C) Text\nAnswer: ", "b"),
                ("Q6: Text must be in closed with?\nA) Four Parentheses B) Two Dots C) Quotation Marks\nAnswer: ", "c"),
                ("Q7: Which of them are correct syntax that uses double quotes inside the parentheses.\nA) print('Hello World!') B) print(Hello,world) C) ('Hello World!')\nAnswer: ", "a"),
                ("Q8: Can you print directly without using quotation marks?\nA) Yes B) No C) Maybe\nAnswer: ", "b"),
                ("Q9: Numbers are used without using?\nA) Text B) Data C) Quotes\nAnswer: ", "c"),
                ("Q10: Do we use quotes for text?\nA) Yes B) No C) Neither\nAnswer: ", "a"),
            ]
#Python Comments
        elif lesson == "4":
            print("""===========================================================================================================================================
                                        PYTHON COMMENTS
            
===========================================================================================================================================
PYTHON COMMENTS
comments ARE IGNORED by Python. they are USED TO EXPLAIN THE CODE.
SINGLI LINE COMMENT        Uses the hash symbol# Comment continues until the end of the line
1 # This is a comment      USED FOR:
2                          * Short explanation
3 print("Hello")           * Disabling a line of code
                           * Quick notes
MULTI-LINE COMMENT
1 ''''''                  Uses triple quotes '''''' comment continues until the closing ''''''.
2 This is                 USED FOR:
3 a multi-line            * Longer explanation  
4 comment.                * Describing functions
5 ''''''                  * Adding documentation
6                         NOTE
7 print("Hello")          The code inside triple quotes is ignored by Python.
==========================================================================================================================================""")
#question for python comment
            questions = [
                ("Q1: What symbol is used for a single line comment?\nA) #  B) // C) **\nAnswer: ", "a"),
                ("Q2: Are comments ignored by Python?\nA) Neither B) Yes C) No\nAnswer: ", "b"),
                ("Q3: What are comments used for?\nA) To delete code  B) To run code C) To explain code\nAnswer: ", "c"),
                ("Q4: What is used for a multi-line comment?\nA) Triple quotes  B) Double quotes C) Single quotes\nAnswer: ", "a"),
                ("Q5: Which one is a comment?\nA) print('Hi') B) # My name is John  C) x = 5\nAnswer: ", "b"),
            ]
#Variables,Constants, and data Types in python            
        elif lesson == "5":
            print("""===========================================================================================================================================
                                        VARIABLES,CONSTANT AND DATA TYPES IN PYTHON
            
===========================================================================================================================================
1.WHAT IS VARIABLE?
A VARIABLE is a named STORAGE LOCATION USED TO KEEP DATA IN A PROGRAM. The value of a variable can change while the program is running.
EXAMPLE: a,b, c, age, name
VARIABLE NAME - age      name - VARIABLE NAME 
STORED VALUE - 20        "John" - STORED VALUE  
VARIABILE NAMING RULES:
A variable can have a SHORT NAME(like x and y) or more DESCRIPTIVE NAME(age,carname,total_volume).
SHORT NAME - are quick to type and often used in simple programs or inside loops.
EXAMPLE: x,y,I,j,n,temp
DESCRIPTIVE NAMES - Clearly explain what the variable stores. They make code easier to read and understandable. 
EXAMPLE: age, carname, total_volume, student_score
REMEMBER:
Both short and descritive names are valid.Choose the one that makes your code clear and easy to understand.
* Use short name for quick,simple tasks or temporary variables.
* Use descriptive names when your code grows or is read by others.
VARIABLE NAMING RULES:
* A variable name MUST START WITH A LETTER or the UNDERSCORE CHARACTER.
EXAMPLE:
age = 20 - Start with a letter
_value = 100 - Start with underscore
total = 50 - Start with a letter
TIPS: After the first character, you can use letters,numbers and underscores.
* A variable name CANNOT START WITH A NUMBER.
EXAMPLE: 
1stValue = 10  - Starts with a number
2Total = 30 - Start with a number
123john = 100 - Start with a number
WHY? Python won't know if it's a variable or a number!
VARIABLE NAMING RULES:
Variables names are CASE-SENSITIVE (age and AGE are two different variables)
Variable 1                     Variable 2             
age                            AGE
18                             25
This is a variable age        This is a variable AGE
GOOD VARIABLE NAMING: 
number - letters,lowercase allowed
NUMBER - Letters,uppercase allowed
spam123 - Letters and numbers allowed
_spped - Underscore allowed
BAD VARIABLE NAMING:
1abc - Cannot start with a number
#bread - Cannot start with a special characters like #
var.12 - Cannot use a special character like . 
space name - Cannot use space
@value - Cannot use speciale character like @
DIFFERENT(CASE-SENSITIVE)
number       Number       NUMBER
value = 10   value = 20   value = 30
*Variable names are CASE-SENSITIVE.These are three different variables.
ASSIGNED VALUE TO VARIABLE - in programming, We store data in variables. We assign a value to a variable using the = (ASSIGMENT OPERATOR).
first_name = ''John'' - VALUE - The data we store in the variable.(can be text,number,etc.) 
|
*VARIABLE NAME*
The name we choose to represent the data (followers naming rules).
*OUTPUT VARIABLES* 
the python PRINT() FUNCTION is often used to output variables.
EXAMPLE:
1 school = ''clark college' - *1.We store the text 'clark college'in a variable named school.
2 print(school) - *2.We use print() to display the value of the variable school.
OUTPUT - clark college - *The value stored in school is displayed.
OUTPUT VARIABLES
in the print() functioon, you output MULTIPLE VARIABLES, SEPARATED BY A COMMA:
========================================================================================================================================== '""")
#Variables,Constants, and data Types in python      
            questions = [
                ("Q1: What is a VARIABLE?\nA) A named storage location used to keep data B) A computer C) A print function\nAnswer: ", "a"),
                ("Q2: Can the value of a variable change?\nA) No B) Yes, it can change C) Only once\nAnswer: ", "b"),
                ("Q3: Which is a SHORT NAME?\nA) student_score B) total_volume C) x\nAnswer: ", "c"),
                ("Q4: Which is a DESCRIPTIVE NAME?\nA) student_score B) x C) y\nAnswer: ", "a"),
                ("Q5: A variable MUST START WITH what?\nA) A number B) A letter or underscore C) A #\nAnswer: ", "b"),
                ("Q6: Which is a CORRECT variable name?\nA) 1abc B) #bread C) _value\nAnswer: ", "c"),
                ("Q7: Are age and AGE the same?\nA) No, they are 2 different variables B) Yes, same C) Maybe\nAnswer: ", "a"),
                ("Q8: What symbol assigns a value?\nA) == B) = C) +\nAnswer: ", "b"),
                ("Q9: In first_name = 'John', what is 'John'?\nA) Variable Name B) Operator C) Value\nAnswer: ", "c"),
                ("Q10: If school = 'clark college', what does print(school) show?\nA) clark college B) school C) print\nAnswer: ", "a"),
            ]
#Basic data types in python            
        elif lesson == "6":
            print("""===========================================================================================================================================
                                        BASIC DATA TYPES ON PYTHON
            
===========================================================================================================================================
*DATA TYPES*
are categories that tell Python what kind of a data a variable stores. They determine the type of value a variable can hold and what operations can be  performed on that value.
123 int - integers numbers - Whole number (no decimal part)"
EXAMPLE: 10, 25, -7 100
3.14 float - Numbers with a decimal point.
EXAMPLE: 12.5, 3.14, -0.00001. 2.0
'' '' str (string or text) - Text or characters inside quotes.
EXAMPLE: '' HELLO'', ''jUAN'', ''CCST''
T/F bool (boolean values) - Represent one of two values: True or False.
EXAMPLE: True, False
*DECLARATION OF VARIABLES*
                       VARIABLE       VALUE      DATA TYPES        DESCRIPTION
name = ''maria''       name         ''Mmria''    str(String)       Stores text inside quotes. 
age = 20               age            20         int(integer)      Stores whole numbers.
grade = 89.5           grade          89.5       float(decimal)    Stores numbers with decimal points.
is_enrolled = True"")  is_enrolled    True       bool(boolean)     Stores True or False value.
==========================================================================================================================================""")
#Basic data types questions
            questions = [
                ("Q1: What are DATA TYPES?\nA) Categories that tell Python what kind of data a variable stores B) A computer C) A print function\nAnswer: ", "a"),
                ("Q2: Which data type is a whole number with NO decimal?\nA) float B) int C) str\nAnswer: ", "b"),
                ("Q3: Which one is a float?\nA) 10 B) ''HELLO'' C) 3.14\nAnswer: ", "c"),
                ("Q4: Which data type is text inside quotes?\nA) str B) int C) bool\nAnswer: ", "a"),
                ("Q5: Which one is a str?\nA) 20 B) ''CCST'' C) True\nAnswer: ", "b"),
                ("Q6: Which data type is True or False only?\nA) int B) float C) bool\nAnswer: ", "c"),
                ("Q7: name = ''maria'', what is the data type of name?\nA) str B) int C) bool\nAnswer: ", "a"),
                ("Q8: age = 20, what is the data type of age?\nA) str B) int C) float\nAnswer: ", "b"),
                ("Q9: grade = 89.5, what is the data type of grade?\nA) int B) str C) float\nAnswer: ", "c"),
                ("Q10: is_enrolled = True, what is the data type?\nA) bool B) int C) str\nAnswer: ", "a"),
            ]
#Arithmetic operators and expressions
        elif lesson == "7":
            print("""===========================================================================================================================================
                                        ARITHMETIC OPERATORS AND EXPRESSIONS
            
===========================================================================================================================================
WHAT ARE ARITHEMETIC OPERATORS?
ARITHMETIC OPERATIORS are symbols used to perform mathematical calculations on numbers. They work the same way as the operators used in everyday mathematics.
EXPRESSIONS IN PYTHON An expression is a combination of values, variable, and operators that evaluates to a result.
*PYTHONS ARITHMETIC OPERATORS*

OPERATORS  DESCRIPTION                                                              EXAMPLE    RESULT       
+          addition (adds value)                                                    5 + 3      8
-          Subraction (Subtracts the second value from the first.)                  10 - 4     6
*          Multiplication (Multiply two values)                                     7 * 2      14
/          Division (Divides two values & returns a decimal.)                       15 / 3     5.0
//         Floor Division (Divides two values and returns the whole number part.)   17 // 3    5
%          modulus (Return the reminder of the division.)                           10 % 3     1
**         Exponentiation (Raises the first value to the power of the second.)       2 ** 3     8 
PYTHON EXAMPLE:l ADD TWO NUMBERS
1 a = 10   #First number
2 b = 5    #Second number
3
4 result = a + b  # add the numbers 
5  print(''The result is:, result)  
                           #display the result
OUTPUT
10 + 5 = 15 THE RESULT IS 15
EXAMPLE OF ADD               
a = 10
b = 5
addition = a + b
print("Addition:", addition) RESULT = 15
EXAMPLE OF SUBTRACTION
a = 10
b = 5
subtraction = a - b
print("Subtraction:", subtraction) RESIULT = 5
EXAMPLPE OF MULTIPLICATION
a = 10
b = 5
multiplication = a * b
print("Multiplication:", multiplication) RESULT = 50
EXAMPLE OF DIVISION
a = 10
b = 5
division = a / b
print("Division:", division) RESULT = 2
EXAMPLE OF FLOOR DIVISION
a = 10
b = 5
floor_division = a // b
print("Floor Division:", floor_division) RESULT = 2
EXAMPLE OF MODULUS
A = 10
B = 5
modulus = A % B
print("Modulus:", modulus) RESULT = 0
EXAMPLE OF EXPONENTIATION
a = 10
b = 5
exponentiation = a ** b
print("Exponentiation:", exponentiation) RESULT = 100000
*EXPRESSION IN PYTHON*                            PEMDAS (Orders of Operations)
Python follows the order of operations (PEMDAS)   P Parentheses      first                  
                                                  E Exponents          |
                                                  M Multiplication     |
                                                  D Division           |
                                                  A Addition           |
                                                  S Subtraction      Last
==========================================================================================================================================""")
#Arithmetic operators and expressions question
            questions = [
                ("Q1: What are ARITHMETIC OPERATORS?\nA) Symbols used to perform mathematical calculations on numbers B) A type of computer C) A print function\nAnswer: ", "a"),
                ("Q2: What is an EXPRESSION in Python?\nA) A computer B) A combination of values, variables, and operators that evaluates to a result C) A print function\nAnswer: ", "b"),
                ("Q3: Which operator is used for 5 + 3?\nA) Subraction B) Addition C) Floor Division\nAnswer: ", "c"),
                ("Q4: Which operator is for SUBTRACTION?\nA) - B) + C) *\nAnswer: ", "a"),
                ("Q5: Which operator is used for 7 * 2?\nA) Addition B) Multiplication C) Subtraction\nAnswer: ", "b"),
                ("Q6: Which operator is used 15 / 3?\nA) Modulus B) Subtraction C) Division\nAnswer: ", "c"),
                ("Q7: Which operator gives the WHOLE NUMBER part only?\nA) // B) / C) %\nAnswer: ", "a"),
                ("Q8: What does % (Modulus) return?\nA) The whole number B) The remainder of the division C) The power\nAnswer: ", "b"),
                ("Q9: Which operation is used 2 ** 3?\nA) floor Division B) Numbers C) Exponentation\nAnswer: ", "c"),
                ("Q10: In PEMDAS, what comes FIRST?\nA) Parentheses B) Addition C) Subtraction\nAnswer: ", "a"),
            ]
#BASIC INPUT AND OUTPUT IN PYTHON
        elif lesson == "8":
            print("""===========================================================================================================================================
                                        BASIC INPUT AND OUTPUT IN PYTHON
            
===========================================================================================================================================
ACCEPTING USER INPUT
purpose of input in programming
Real-life analogies (e.g., asking for user's name and responding
EXAMPLE:
ACCEPTING USER INPUT
PYTHONS INPUT - GETTING USER INPUT
1 name = input(''Enter your name:'')
2 age = input(''Enter you age:'')
*Using input()function
*Syntax: variable = input("Prompt message:'')
*All input is string type by default
FORMATING OUTPUT
Using comma , in print():
PYTHON INPUT - GETTING USER INPUT AND DISPLAYING OUTPUT
1 name = input(''Enter Name:'')
2 age = input(''Enter Age:'')
3 print(''Name:'', name)
4 print(''Age:'', age)
CONVERTING INPUT TO OTHER DATA TYPES
B. Float Input (for decimal numbers)
PYTHON CODE
1 grade = float(input("Enter your grade: "))
2 print(f''Your grade is {grade)'')
CONVERTING INPUT TO OTHER DATA TYPES
C. Boolean Input (True or False using conditions)
PYTHON CODE
1 answer = input("Are you a student? (yes/no): ")
2 is_student = answer.lower() == "yes"
3 print("Student status:", is_student)
CONVERTING INPUT TO OTHER DATA TYPES
Example Program (Combining All)
PYTHON CODE
1 name = input("Enter your name: ")
2 age = int(input("Enter your age: "))
3 grade = float(input("Enter your final grade: "))
4 print(f"Student: {name), Age: {age), Final Grade: {grade)
==========================================================================================================================================""")
#BASIC INPUT AND OUTPUT IN PYTHON QUESTION
            questions = [
                ("Q1: What is the PURPOSE of input()?\nA) To ask the user for information and use it in the program B) To print only C) To delete data\nAnswer: ", "a"),
                ("Q2: What is the SYNTAX of input()?\nA) print(''Hello'') B) variable = input(''Prompt message:'') C) variable = 10\nAnswer: ", "b"),
                ("Q3: By default, what data type is ALL input?\nA) int B) float C) str (string)\nAnswer: ", "c"),
                ("Q4: How do you print Name and Age with a comma?\nA) print(''Name:'', name) B) print(name) C) input(name)\nAnswer: ", "a"),
                ("Q5: How do you convert input to an INTEGER?\nA) str(input()) B) int(input(''Enter your age: '')) C) float(input())\nAnswer: ", "b"),
                ("Q6: How do you convert input to a FLOAT?\nA) int(input()) B) str(input()) C) float(input(''Enter your grade: ''))\nAnswer: ", "c"),
                ("Q7: Is this correct grade = float(input(''Enter your grade: ''))?\nA) Yes B) No C) Neither\nAnswer: ", "a"),
            ]
#PARAMA STOP              
        elif lesson == "0":
            print("Exit!")
            break
#BABALIK SA MENU            
        else:
            print("""Back to main menu! 
YOU HAVE TO CHOSE  AGAIN BETWEEN PRELIM,MIDTERM AND FINAL!!!""")
            continue
#MIDTERM            
    elif major == "2":
        print("""1 - CONDITIONAL STATEMENTS IN PYTHON
2 - LOGICAL OPERATOR
0 - EXIT""")
        lesson = input("CHOSE A LESSON (0-2): ").strip()
#CONDITIONAL STATEMENTS IN PYTHON       
        if lesson == "1":
            print("""===========================================================================================================================================
                                        CONDITIONAL STATEMENTS IN PYTHON
            
===========================================================================================================================================
2. INTRODUCTION TO CONDITIONAL STATEMENTS
A conditional statement allows a program to make decisions based on whether a condition is True or False.

BASIC STRUCTURE
if condition:
    statement
if - The if keyword starts the conditional statement.
condition - The condition is evaluated. If it is True, the indented statement is executed.
statement - The statement is the code that runs when the condition is True.

HOW IT WORKS
Start -> Is the condition True? -> Yes (True) -> Execute the statement -> End
Start -> Is the condition True? -> No (False) -> Skip the statement -> End

EXAMPLE
age = 18
if age >= 18:
    print("You are an adult.")
Output when run:
You are an adult.

In simple terms...
The program checks the condition.
If True, it does something.
If False, it does nothing (or something else).
---
3. RELATIONAL OPERATORS
Relational operators, also called comparison operators, are used to compare two values. The result is always either True or False.

Operator    Meaning                    Example    Result
==          Equal to                   10 == 10   True
!=          Not equal to               10 != 5    True
>           Greater than               10 > 5     True
<           Less than                  5 < 10     True
>=          Greater than or equal to   10 >= 10   True
<=          Less than or equal to      5 <= 10    True

REMEMBER: Relational operators compare values and always return either True or False.

EXAMPLE:
score = 85
print(score >= 75)
Output: True
Explanation: Since 85 is greater than or equal to 75, the expression score >= 75 evaluates to True.
---
COMPARISON OPERATORS
> Greater than
< Less than
>= Greater than or equal to
<= Less than or equal to
== Equal to
!= Not equal to
---
4. The if Statement 
The if statement executes a block of code only when a condition is true.
SYNTAX
if condition:
    statement(s)
if - The if keyword starts the statement.
condition - The condition is evaluated. If it is True, the indented block is executed.
statement(s) - One or more statements that run when the condition is True.

HOW IT WORKS
Start -> Is the condition True? -> Yes (True) -> Execute the indented block -> End
Start -> Is the condition True? -> No (False) -> Skip the block -> End

If the condition is False, the indented block is skipped.

EXAMPLE
age = 20
if age >= 18:
    print("You are an adult.")

WHAT HAPPEN?
If age is 18 or more (True), the message is printed.
If age is less than 18 (False), nothing happens.

KEY POINTS
The block of code must be indented.
The block runs only when the condition is True.
---
5. The if-else Statement
The else statement provides an alternative when the if condition is false.

SYNTAX
if condition:
    statement
else:
    statement

KKEY POINTS
Use else when you want an alternative action if the if condition is False.
Only one of the if or else block will be executed.

EXAMPLE
score = 65
if score >= 75:
    print("Passed")
else:
    print("Failed")
Output: Failed
Explanation: In this example, score is 65, which is less than 75, so the else block runs and the program prints Failed.
---
5. The if-else Statement (with All Comparison Operators)
The else statement provides an alternative when the if condition is false.
SYNTAX
if condition:
    statement
else:
    statement

KEY POINTS
The if block runs when the condition is True.
The else block runs when the condition is False.
Only one of the blocks will be executed.

EXAMPLE
score = 65
if score >= 75:
    print("Passed")
else:
    print("Failed")
Output: Failed

EXAMPLE of if-else with All Comparison Operators
Operator   Meaning                    Condition Example   When True(OUTPUT)  When False(OUTPUT)
==         Equal to                   score == 10         Equal              Not Equal
!=         Not equal to               score != 10         Not Equal          Equal
>          Greater than               score > 10          Greater            Not Greater
<          Less than                  score < 10          Less               Not Less
>=         Greater than or equal to   score >= 10         Greater or Equal   Less
<=         Less than or equal to      score <= 10         Less or Equal      Greater

CODE EXAMPLE (score = 10)
if score == 10: print("Equal") else: print("Not Equal")
if score != 10: print("Not Equal") else: print("Equal")
if score > 10: print("Greater") else: print("Not Greater")
if score < 10: print("Less") else: print("Not Less")
if score >= 10: print("Greater or Equal") else: print("Less")
if score <= 10: print("Less or Equal") else: print("Greater")

REMEMBER
A condition is either True or False.
The program chooses one path:
If the condition is True -> if block
If the condition is False -> else block
if else - Make decisions in your code!
---
6. The if-elif-else Statement
The elif statement is used when there are multiple conditions to evaluate. Python checks each condition from top to bottom and executes the first condition that is True.

SYNTAX
if condition1:
    statement
elif condition2:
    statement
else:
    statement

KEY POINTS
Python checks conditions from top to bottom.
If a condition is True, its block is executed and the rest are skipped.
If none of the conditions are True, the else block is executed.

EXAMPLE
score = 85
if score >= 90:
    print("Excellent")
elif score >= 80:
    print("Very Good")
elif score >= 75:
    print("Passed")
else:
    print("Failed")
Output: Very Good

EXPLANATION
score is 85
85 >= 90 -> False
85 >= 80 -> True
Therefore, print("Very Good") is executed.
The remaining elif and else blocks are skipped.

In an if-elif-else structure, only the first condition that evaluates to True is executed.
---
NESTED CONDITION IN PYTHON
A nested condition is a condition inside another condition.

SYNTAX
if condition1:
    if condition2:
        # block of code
    else:
        # block of code
else:
        # block of code
KEY POINTS        
First condition is checked.
Second condition is checked only if the first condition is True.
This runs if the first condition is False.

CODE
gender = input("Enter gender (M/F): ")
age = int(input("Enter age: "))
if gender == "M":
    if age >= 21:
        print("You are a MALE DEBUTANT.")
    else:
        print("You are a male, but not a debutant yet.")
else:
    if age >= 18:
        print("You are a FEMALE DEBUTANT.")
    else:
        print("You are a female, but not a debutant yet.")

DEBUTANT AGE RULES BY GENDER
A debutant is someone (male or female) who meets the minimum age requirement and is being formally presented in a debut.
Start -> What is your gender?
Male (M) -> Is age >= 21? -> Yes -> You are a MALE DEBUTANT.
Male (M) -> Is age >= 21? -> No -> You are a male, but not a debutant yet.
Female (F) -> Is age >= 18? -> Yes -> You are a FEMALE DEBUTANT.
Female (F) -> Is age >= 18? -> No -> You are a female, but not a debutant yet.
-> End

SAMPLE RUNS
1. Enter gender (M/F): M / Enter age: 21 -> You are a MALE DEBUTANT.
2. Enter gender (M/F): M / Enter age: 19 -> You are a male, but not a debutant yet.
3. Enter gender (M/F): F / Enter age: 18 -> You are a FEMALE DEBUTANT.
4. Enter gender (M/F): F / Enter age: 16 -> You are a female, but not a debutant yet.

TIP: Read the flow from the top. The inner condition (age) is checked only if the outer condition (gender) is True.
==========================================================================================================================================""")
#CONDITIONAL STATEMENTS IN PYTHON QUESTION
            questions = [
                ("Q1: What is if for?\nA) If True, do it B) To delete C) To print only\nAnswer: ", "a"),
                ("Q2: What is else for?\nA) To stop B) If False, do the other one C) To add\nAnswer: ", "b"),
                ("Q3: What does == mean?\nA) Add B) Greater C) Equal to\nAnswer: ", "c"),
                ("Q4: What does > mean?\nA) Greater than B) Equal C) Less than\nAnswer: ", "a"),
                ("Q5: What does != mean?\nA) Equal B) Not equal to C) Greater\nAnswer: ", "b"),
                ("Q6: What is 20 == 20?\nA) False B) 20 C) True\nAnswer: ", "c"),
                ("Q7: What is elif for?\nA) Check many conditions, do first True one B) Stop C) Print\nAnswer: ", "a"),
                ("Q8: If score = 65, if score >= 75: Passed else: Failed. What prints?\nA) Passed B) Failed C) 65\nAnswer: ", "b"),
                ("Q9: What is nested if?\nA) Print B) Add C) If inside if\nAnswer: ", "c"),
                ("Q10: What do you call this operator >=?\nA) Greater thatn or Equal to B) Less that or Equal to C) Equal\nAnswer: ", "a"),
            ]
#LOGICAL OPERATOR
        elif lesson == "2":
            print("""===========================================================================================================================================
                                        LOGICAL OPERATOR
            
===========================================================================================================================================
PYTHON LESSON: LOGICAL OPERATORS

LEARNING OBJECTIVES
At the end of the lesson, students should be able to:
1 Define logical operators in Python.
2 Identify the three logical operators: and, or, and not.
3 Use logical operators with conditional statements.
4 Combine multiple conditions in a Python program.
5 Create simple real-life programs using logical operators.
---
WHAT ARE LOGICAL OPERATORS?
Logical operators are used to combine or reverse conditions in a Python program.
They are commonly used with if, elif, and else.

Python has three logical operators:
Operator - Meaning
and - Both conditions must be True
or - At least one condition must be True
not - Reverses the result

Example:
age = 20
if age >= 18 and age <= 60:
    print("Allowed")

Here, Python checks two conditions:
1 age >= 18
2 age <= 60
Both must be True because we used and.
---
The and Operator
The and operator returns True only when ALL conditions are True.

EXAMPLE:
age = 20
has_id = True
if age >= 18 and has_id:
    print("You are allowed to enter.")
else:
    print("You are not allowed to enter.")

EXPLANATION:
The program checks:
1 age >= 18 -> True
2 has_id -> True
Since both are True:
True and True = True
---
Truth Table - and
Condition A  Condition B   A and B
True         True          True
True         False         False
False        True          False
False        False         False

Easy way to remember:
AND = KAILANGAN LAHAT TRUE
---
The or Operator
The or operator returns True when at least ONE condition is True.

EXAMPLE CODE:
day = "Saturday"
if day == "Saturday" or day == "Sunday":
    print("It's the weekend!")
else:
    print("It's a regular school day.")

THE PROGRAM CHECKS:
1 day == "Saturday" -> True
2 day == "Sunday" -> False
Therefore:
True or False = True
Output:
It's the weekend!
---
Truth Table - or
Condition A   Condition B   A or B
True          True          True
True          False         True
False         True          True
False         False         False

Easy way to remember:
OR = KAHIT ISA LANG TRUE
---
THE NOT OPERATOR
The not operator reverses the result of a condition.
True -> False
False -> True

EXAMPLE:
is_raining = False
if not is_raining:
    print("You can go outside.")
else:
    print("Bring an umbrella.")

EXPLANATION:
1 is_raining = False
2 not is_raining
3 not False = True
4 Output: You can go outside.
---
Truth Table - not
Condition   not Condition
True        False
False       True

Easy way to remember:
NOT = BALIKTARIN ANG RESULT
==========================================================================================================================================""")  
#LOGICAL OPERATOE QUESTIONS
            questions = [
                ("Q1: What are LOGICAL OPERATORS used for?\nA) To combine or reverse conditions B) To print only C) To delete data\nAnswer: ", "a"),
                ("Q2: How many logical operators are there in Python?\nA) 2 B) 3 (and, or, not) C) 5\nAnswer: ", "b"),
                ("Q3: What does AND mean?\nA) One is True B) Reverses C) Both conditions must be True\nAnswer: ", "c"),
                ("Q4: What is True and True?\nA) True B) False C) Error\nAnswer: ", "a"),
                ("Q5: What is True and False?\nA) True B) False C) True and False\nAnswer: ", "b"),
                ("Q6: What does OR mean?\nA) Both must be True B) Reverses C) At least ONE must be True\nAnswer: ", "c"),
                ("Q7: What is False or True?\nA) True B) False C) Error\nAnswer: ", "a"),
                ("Q8: What is False or False?\nA) True B) False C) Error\nAnswer: ", "b"),
                ("Q9: What does NOT do?\nA) Adds B) Multiplies C) Reverses the result\nAnswer: ", "c"),
                ("Q10: What is not False?\nA) True B) False C) Error\nAnswer: ", "a"),
            ]
#PARAMA STOP              
        elif lesson == "0":
            print("Exit!")
            break
#BABALIK SA MENU            
        else:
            print("""Back to main menu! 
YOU HAVE TO CHOSE  AGAIN BETWEEN PRELIM,MIDTERM AND FINAL!!!""")
            continue
#FINALS INTRODUCTION TO ITERATION AND LOOPS        
    if major == "3":
        print("""1 - INTRODUCTION TO ITERATION AND LOOPS 
0 - EXIT""")
        lesson = input("CHOSE 1 TO GO TO LESSON IN FINALS AND 0 TO EXIT: ").strip()
        if lesson == "1":
            print("""===========================================================================================================================================
                                        INTRODUCTION TO ITERATION AND LOOPS 
            
===========================================================================================================================================
Iteration means repeating a process. In programming, it means repeatedly executing a set of instructions. Each repetition is called an iteration.
for number in range(3):
    print("Welcome to Python!")

OUTPUT:
1. Welcome to Python!
2. Welcome to Python!
3. Welcome to Python!

The print() instruction executes once during each iteration.
---
Iteration allows a program to perform the same task multiple times.

Without a loop, instructions must be written repeatedly:

Without a loop:
print("Study Python")
print("Study Python")
print("Study Python")
print("Study Python")

Using a loop:
for number in range(4):
    print("Study Python")

Both programs produce the same output, but the loop makes the program shorter and easier to modify. To repeat the message 100 times, change 4 to 100.
---
TYPE OF LOOPS IN PYTHON
Python has two main types of loops: for and while.

for loop
Repeats instructions for each item in a sequence. Useful when the number of repetitions is known.
for number in range(3):
    print("Hello!")
1. Hello! -> 2. Hello! -> 3. Hello!

while loop
Repeats instructions while a condition is True. Useful when repetition depends on a condition.
count = 1
while count <= 3:
    print("Hello!")
    count += 1
Check condition -> Repeat
Both examples print Hello! three times.
---
PYTHON for Loop

SYNTAX
for variable in sequence:
    statement(s)

VARIABLE: receives each item
SEQUENCE: items to loop through
INDENTED STATEMENT: the loop body

EXAMPLE CODE
for number in range(4):
    print("Study Python")

This loop prints Study Python four times.
Use a colon (:) after the loop header and indent the loop body.
---
for Loop: Print Numbers 1 to 5

EXAMPLE CODE
for number in range(1, 6):
    print(number)

OUTPUT
1
2
3
4
5

HOW IT WORKS
1. range(1, 6) produces 1, 2, 3, 4, and 5.
2. The start value 1 is included; the stop value 6 is excluded.
3. Each iteration assigns the next value to number.
4. print(number) displays that value. After 5, the loop ends.
5 iterations: 1 -> 2 -> 3 -> 4 -> 5
---
Counting Downward with range(): 5 to 1

EXAMPLE CODE
for number in range(5, 0, -1):
    print(number)

OUTPUT
5
4
3
2
1

HOW IT WORKS
1. Start at 5.
2. Stop before 0; the stop value is excluded.
3. The step -1 decreases the value by 1 each iteration.
4. print(number) displays 5, 4, 3, 2, and 1 on separate lines.
5 iterations: 5 -> 4 -> 3 -> 2 -> 1

---
PYTHON while Loop

SYNTAX
while condition:
    statement(s)

condition: checked before each iteration
Indented statements: run while the condition is True.

EXAMPLE CODE
count = 1
while count <= 5:
    print(count)
    count += 1

This loop prints the numbers 1 to 5.

count += 1 increases count by 1 each iteration. When count becomes 6, the condition is False and the loop stops.
---
COUNTING DOWNWARD WITH A While Loop: 5 to 1

EXAMPLE CODE
number = 5
while number >= 1:
    print(number)
    number -= 1

OUTPUT
5
4
3
2
1

HOW IT WORKS
1. Start with number = 5.
2. Repeat while number >= 1.
3. Print number, then decrease it by 1 using number -= 1.
4. Stop when number becomes 0 and the condition is False.
5 iterations: 5 -> 4 -> 3 -> 2 -> 1
---
REPEATING A PROGRAM WITH While True

EXAMPLE CODE
while True:
    name = input("Enter your name (X to exit): ")
    if name.upper() == "X":
        print("Program stopped.")
        break
    print("Hello,", name)

SAMPLE OUTPUT
Enter your name (X to exit): Ana
Hello, Ana
Enter your name (X to exit): Mark
Hello, Mark
Enter your name (X to exit): X
Program stopped.

HOW IT WORK
1. while True keeps the program repeating.
2. Enter a name to display a greeting.
3. Type X or x, then press Enter. break stops the loop.

The program repeats until the user chooses to exit.
==========================================================================================================================================""")
#INTRODUCTION TO ITERATION AND LOOP QUESTION
            questions = [
                ("Q1: What does ITERATION mean?\nA) Repeating a process B) Deleting a process C) Stopping a process\nAnswer: ", "a"),
                ("Q2: What is each repetition called?\nA) Loop B) Iteration C) Variable\nAnswer: ", "b"),
                ("Q3: Which loop is used when number of repetitions is known?\nA) while loop B) if loop C) for loop\nAnswer: ", "c"),
                ("Q4: Which loop repeats while condition is True?\nA) while loop B) for loop C) if loop\nAnswer: ", "a"),
                ("Q5: Which loop will print Hello 3 times if you know it is 3 times?\nA) if loop B) for loop C) while True loop only\nAnswer: ", "b"),
                ("Q6: What will happen if you forget count += 1 in a while loop?\nA) It will stop B) It will print once C) It will loop forever / infinite loop\nAnswer: ", "c"),
                ("Q7: What does count += 1 do?\nA) Increases count by 1 B) Decreases count by 1 C) Stops the loop\nAnswer: ", "a"),
                ("Q8: In while True program, what stops the loop?\nA) print B) break C) input\nAnswer: ", "b"),
                ("Q9: What do you put after for and while header?\nA) Semicolon ; B) Comma , C) Colon :\nAnswer: ", "c"),
                ("Q10: Which loop is best to repeat a program until user types X to exit?\nA) while True loop B) for loop with range(3) C) if loop\nAnswer: ", "a"),
            ]
        else:
            print("Exit!")
            break
#EXIT PAG NAG EXIT SYA SA PRELIM,MIDTERM AND FINALS            
    elif major == "0":
        print("THANK YOU FOR TRYING PYTHON TUTORIAL!")
        break
#PARA SA QUESTION AND ANSWER
    total_lives = 3
    streak = 0
    game_over = False
    print(f"\nYou have {total_lives} LIVES: ❤️❤️❤️")

    for question, correct_answer in questions:
        lives_this_question = 3
        while True:
            print(f"Total Lives: {'❤️' * total_lives} ({total_lives}) | Tries: {'❤️' * lives_this_question} ({lives_this_question}) | Streak: {streak}")
            answer = input(question).lower().strip()
            if answer == correct_answer:
                print("Correct! Next question!\n")
                streak += 1
                if streak == 3:
                    total_lives += 1
                    print("STREAK BONUS! +1 LIFE!")
                    streak = 0
                break
            else:
                lives_this_question -= 1
                total_lives -= 1
                streak = 0
                print(f"Wrong! You lost 1 life! Total Lives left: {total_lives}\n")
                if lives_this_question == 0:
                    print("You used all 3 tries! GAME OVER!")
                    game_over = True
                    break
                if total_lives == 0:
                    print("GAME OVER! You ran out of total lives!")
                    game_over = True
                    break
        if game_over:
            break

    if not game_over:
        print("=" * 40)
        print("CONGRATS! You finished this lesson!")
        print(f"You finished with {total_lives} lives left!")
        print("=" * 40)

    while True:
        again = input("\nDo you want to try another lesson? (Y/N): ").upper().strip()
        if again == "Y":
            break
        elif again == "N":
            print(F"Thanks for playing {name}!!!")
            exit()
        else:
            print("Please type Y or N only!")
