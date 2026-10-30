from idlelib.configdialog import changes

print("==============================================")
print("                 FM GROCERY                   ")
print("==============================================\n")
print("[PRODUCTS]                    DATE: 12/3/24")
print("\n-----------------CANNED-----------------")
print("[1]Corned Beef (150g)            - P70.12")
print("[2]555 Tuna (155g)               - P45.23")
print("[3]Century Tuna (155)            - P75.11")

print("\n----------------PASTRIES----------------")
print("[4]Gardenia Classic WB (600g)    - P90.42")
print("[5]Gardenia High Fiber WB (400g) - P93.76")
print("[6]SariMonde Tasty Bread (450g)  - P91.12")

print("\n-----------------SNACKS-----------------")
print("[7]Nagaraya (160g)               - P49.42")
print("[8]Potato Fries Ketchup (35g)    - P65.59")
print("[9]Oishi Pillows Choco (38g)     - P14.21")

print("\n-----------------ALCOHOL----------------")
print("[10]Alfonso Light (1L)           - P290.42")
print("[11]Alfonso Platinum (1L)        - P380.53")
print("[12]RedHorse (100ml)             - P90.21")
print("\n==============================================\n")

num = int(input("Product Number: "))

if num == 1:
    product = "Corned Beef (150g)"
    price = 70.12

elif num == 2:
    product = "555 Tuna (155g)"
    price = 45.23

elif num == 3:
    product = "Century Tuna (155g)"
    price = 75.11

elif num == 4:
    product = "Gardenia Classic WB (600g)"
    price = 90.42

elif num == 5:
    product = "Gardenia High Fiber WB (400g)"
    price = 93.76

elif num == 6:
    product = "SariMonde Tasty Bread (450g)"
    price = 91.12

elif num == 7:
    product = "Nagaraya (160g)"
    price = 49.42

elif num == 8:
    product = "Potato Fries Ketchup (35g)"
    price = 65.59

elif num == 9:
    product = "Oishi Pillows Choco (38g)"
    price = 14.21

elif num == 10:
    product = "Alfonso Light (1L)"
    price = 290.42

elif num == 11:
    product = "Alfonso Platinum (1L)"
    price = 380.53

elif num == 12:
    product = "RedHorse (100ml)"
    price = 90.21
else:
    print("Invalid Input.")
    exit()

q = int(input("Quantity: "))

if q <= 0:
    print("Invalid Quantity.")
    exit()

subt = price * q

if subt >= 1500:
    dis = 0.25
elif subt >= 1000:
    dis = 0.20
elif subt >= 500:
    dis = 0.10
else:
    dis = 0

disc = subt * dis
dis_amt = subt - disc
tx = dis_amt * 0.12
ftot = dis_amt + tx

print("\n==============================================")
print("                   RECEIPT                   ")
print("==============================================\n")
print(f"Product Number : {num}")
print(f"Price          : P{price}")
print(f"Quantity       : {q:.0f}")
print("==============================================")
print(f"Subtotal       : P{subt:.2f}")
print(f"Discount       : P{disc:.2f}")
print(f"Taxe           : P{tx:.2f}")
print("==============================================")
print(f"Total          : P{ftot:.2f}")
print("==============================================")

paym = float(input("Enter your Payment: P"))

if paym >= ftot:
    change = paym - ftot
    print(f"Payment : P{paym:.2f}")
    print(f"Change  : P{change:.2f}")
else:
    balance = ftot - paym
    print(f"Insufficient Balance.")
























    print("="*60)
print("                WELCOME TO PYTHON TUTORIAL! ")
print("="*60)

name = input("Enter your name: ")
print(" ")
print(f"Welcome, {name}!")
print("what do you want to learn?")
print(" ")

print("[1]  Variables")
print("[2]  Data types")
print("[3]  Python syntax")
print("[4]  Print statement")
print("[5]  Print text")
print("[6]  Printing numbers")
print("[7]  Python comments")
print("[8]  Variable naming rules")
print("[9]  Assigned value to variable")
print("[10] Declaration of variables")
print("[11] Assign value and output the value")
print("[12] Arithmetic operators")
print("[13] Expression in python")
print("[14] Basic input and output in python")
print("[15] Converting input to other data types")
print("[16] Conditional statement in python")
print("[17] Nested condition in python")
print("[18] Logical operators")
print("[19] Iteration")
print("[20] Types of loops in python")

print("[0] Exit")

print(" ")
print("="*60)
print(" ")

print(" ")
choice = input("Enter yout choice: ")

if choice == "1":
    print("LESSON 1: Variables")
    print("DEFINITION:")
    print("A variable is a container used to store data.")
    print("EXPLANATION:")
    print("Variables store information such as names and numbers.")
    print("EXAMPLE:")
    print('name = "John"')
    print("age = 20")
    print("print(name)")
    print("print(age)")
    print("OUTPUT:")
    print("John")
    print("20")

elif choice == "2":
    print("LESSON 2: DATA TYPES")
    print("DEFINITION:")
    print("Data types identify the kind of data stored in a variable.")
    print("EXPLANATION:")
    print("Examples are int, float, str, and bool.")
    print("EXAMPLE:")
    print('age = 20')
    print('name = "John"')
    print("print(type(age))")
    print("print(type(name))")
    print("OUTPUT:")
    print("<class 'int'>")
    print("<class 'str'>")

elif choice == "3":
    print("LESSON 3: PYTHON SYNTAX")
    print("DEFINITION:")
    print("Syntax refers to the rules for writing Python code.")
    print("EXPLANATION:")
    print("Python code must follow correct writing rules.")
    print("EXAMPLE:")
    print('print("Hello World")')
    print("OUTPUT:")
    print("Hello World")

elif choice == "4":
    print("LESSON 4: PRINT STATEMENT")
    print("DEFINITION:")
    print("The print() function displays information on the screen.")
    print("EXPLANATION:")
    print("It can display text, numbers, and variables.")
    print("EXAMPLE:")
    print('print("Welcome to Python")')
    print("OUTPUT:")
    print("Welcome to Python")

elif choice == "5":
    print("LESSON 5: PRINT TEXT")
    print("DEFINITION:")
    print("Print text means displaying words or sentences.")
    print("EXPLANATION:")
    print("Text must be enclosed in quotation marks.")
    print("EXAMPLE:")
    print('print("I love Python")')
    print("OUTPUT:")
    print("I love Python")

elif choice == "6":
    print("LESSON 6: PRINTING NUMBERS")
    print("DEFINITION:")
    print("Python can display numbers using print().")
    print("EXPLANATION:")
    print("Numbers do not need quotation marks.")
    print("EXAMPLE:")
    print("print(100)")
    print("print(50 + 25)")
    print("OUTPUT:")
    print("100")
    print("75")

elif choice == "7":
    print("LESSON 7: PYTHON COMMENTS")
    print("DEFINITION:")
    print("Comments are notes that Python does not execute.")
    print("EXPLANATION:")
    print("A comment starts with the # symbol.")
    print("EXAMPLE:")
    print('# This is a comment')
    print('print("Hello")')
    print("OUTPUT:")
    print("Hello")

elif choice == "8":
    print("LESSON 8: VARIABLE NAMING RULES")
    print("DEFINITION:")
    print("Variable names identify stored values.")
    print("EXPLANATION:")
    print("Names cannot start with a number or contain spaces.")
    print("EXAMPLE:")
    print('student_name = "Alex"')
    print("age = 18")
    print("OUTPUT:")
    print("student_name = Alex")
    print("age = 18")

elif choice == "9":
    print("LESSON 9: ASSIGNED VALUE TO VARIABLE")
    print("DEFINITION:")
    print("Assignment means giving a value to a variable.")
    print("EXPLANATION:")
    print("The equal sign 😊) assigns a value.")
    print("EXAMPLE:")
    print("score = 95")
    print("print(score)")
    print("OUTPUT:")
    print("95")

elif choice == "10":
    print("LESSON 10: DECLARATION OF VARIABLES")
    print("DEFINITION:")
    print("A variable is created when you assign a value to it.")
    print("EXPLANATION:")
    print("Python does not require a separate declaration keyword.")
    print("EXAMPLE:")
    print('name = "Maria"')
    print("number = 10")
    print("OUTPUT:")
    print("Maria")
    print("10")

elif choice == "11":
    print("LESSON 11: ASSIGN VALUE AND OUTPUT THE VALUE")
    print("DEFINITION:")
    print("This means storing a value and displaying it.")
    print("EXPLANATION:")
    print("Use = to assign a value and print() to display it.")
    print("EXAMPLE:")
    print('city = "Manila"')
    print("print(city)")
    print("OUTPUT:")
    print("Manila")

elif choice == "12":
    print("LESSON 12: ARITHMETIC OPERATORS")
    print("DEFINITION:")
    print("Arithmetic operators perform mathematical calculations.")
    print("EXPLANATION:")
    print("Examples are +, -, *, and /.")
    print("EXAMPLE:")
    print("print(10 + 5)")
    print("print(10 - 5)")
    print("print(10 * 2)")
    print("OUTPUT:")
    print("15")
    print("5")
    print("20")

elif choice == "13":
    print("LESSON 13: EXPRESSION IN PYTHON")
    print("DEFINITION:")
    print("An expression combines values and operators.")
    print("EXPLANATION:")
    print("Python evaluates expressions to produce a result.")
    print("EXAMPLE:")
    print("result = 10 + 5 * 2")
    print("print(result)")
    print("OUTPUT:")
    print("20")

elif choice == "14":
    print("LESSON 14: BASIC INPUT AND OUTPUT")
    print("DEFINITION:")
    print("Input receives information and output displays information.")
    print("EXPLANATION:")
    print("input() receives data while print() displays data.")
    print("EXAMPLE:")
    print('name = input("Enter name: ")')
    print('print("Hello", name)')
    print("OUTPUT:")
    print("Enter name: Alex")
    print("Hello Alex")

elif choice == "15":
    print("LESSON 15: CONVERTING INPUT TO OTHER DATA TYPES")
    print("DEFINITION:")
    print("Type conversion changes a value into another data type.")
    print("EXPLANATION:")
    print("int(), float(), and str() are used for conversion.")
    print("EXAMPLE:")
    print('age = int("20")')
    print("print(age + 5)")
    print("OUTPUT:")
    print("25")

elif choice == "16":
    print("LESSON 16: CONDITIONAL STATEMENT")
    print("DEFINITION:")
    print("A conditional statement allows a program to make decisions.")
    print("EXPLANATION:")
    print("if and else execute code depending on a condition.")
    print("EXAMPLE:")
    print("age = 18")
    print("if age >= 18:")
    print('    print("Adult")')
    print("else:")
    print('    print("Minor")')
    print("OUTPUT:")
    print("Adult")

elif choice == "17":
    print("LESSON 17: NESTED CONDITION")
    print("DEFINITION:")
    print("A nested condition is an if statement inside another if.")
    print("EXPLANATION:")
    print("It checks another condition inside an existing condition.")
    print("EXAMPLE:")
    print("age = 20")
    print("if age >= 18:")
    print("    if age >= 20:")
    print('        print("20 or older")')
    print("OUTPUT:")
    print("20 or older")

elif choice == "18":
    print("LESSON 18: LOGICAL OPERATORS")
    print("DEFINITION:")
    print("Logical operators combine or reverse conditions.")
    print("EXPLANATION:")
    print("The three main operators are and, or, and not.")
    print("EXAMPLE:")
    print("print(True and True)")
    print("print(True or False)")
    print("print(not True)")
    print("OUTPUT:")
    print("True")
    print("True")
    print("False")

elif choice == "19":
    print("LESSON 19: ITERATION")
    print("DEFINITION:")
    print("Iteration means repeating a set of instructions.")
    print("EXPLANATION:")
    print("Loops allow code to run multiple times.")
    print("EXAMPLE:")
    print("for i in range(3):")
    print("    print(i)")
    print("OUTPUT:")
    print("0")
    print("1")
    print("2")

elif choice == "20":
    print("LESSON 20: TYPES OF LOOPS IN PYTHON")
    print("DEFINITION:")
    print("Python has two main types of loops: for and while.")
    print("EXPLANATION:")
    print("A for loop repeats over a sequence.")
    print("A while loop repeats while a condition is true.")
    print("EXAMPLE:")
    print("for i in range(3):")
    print('    print("Hello")')
    print("OUTPUT:")
    print("Hello")
    print("Hello")
    print("Hello")

else:
    print("Invalid choice! Please select from 1 to 20.")

    print(f"Balance : {balance:.2f}")
print("\n----------THANKYOU FOR YOUR PURCHASE----------")
