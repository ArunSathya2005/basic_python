# Basic_python
PYTHON VARIABLES AND DATA TYPES
    - HI Welcome! If you're just starting out python. This guide will give you a quick overview of the fundamentals. 
   -  Python is a powerfull,readable, and beginner-friendly programming language used in web development,AI,
   -  Data science and more.

1) why python
Simple and readable: beginner friendly syntax
                   Stron community: Supportive and active developer base
                   Massive ecosystem: Thousands of libraries and frameworks


Commom libraries

                     
Area                                         popular libraries

Web development                              django,Flask,fastApi
data science                                 pandas,Numpy,Matplotlib
Machine learning                             scikit-learn,Pytorch,TensorFlow
Automation                                   Requestes,selenium,Pyautogui
                     
HELLO WORLD EXAMPLE 

python
print ("hello world")


---
                                

 ##  Python Variables

 In Python, **variables** are used to store data that can be referenced and manipulated later in your code.
 You don’t need to declare the type—Python is **dynamically typed**, so it figures it out for you.

  Creating Variables

  python
      name = "Arun"       # string
      age = 20             # integer
      height = 5.6         # float
      is_student = True    # boolean

Python uses `=` to assign values.


  Rules for Variable Names

* Must start with a **letter** or an **underscore (`_`)**
*  Cannot start with a number
* Can contain letters, numbers, and underscores
* Are **case-sensitive** (`Name` and `name` are different)

  Valid:

   python
         user_name = "Bob"
          _age = 30


  Invalid:

 python
 2name = "Error"     # starts with number
  user-name = "Error" # hyphen not allowed




  Reassigning & Dynamic Typing

 Variables can change type at runtime:

 python
                              
  x = 42       # int
  x = "hello"  # now it's a string

 Variable Types (Built-in)

| Type    | Example                  |
| ------- | ------------------------ |
| `int`   | `x = 10`                 |  
| `float` | `pi = 3.14`              |
| `str`   | `name = "Eve"`           |
| `bool`  | `is_valid = True`        | 
| `list`  | `nums = [1, 2, 3]`       |
|  `dict` | `user = {"name": "Max"}` |


Best Practices

* Use **meaningful names** (e.g. `user_age` instead of `ua`)
* Use **snake\_case** for variable names
* Avoid using Python **keywords** as variable names (e.g. `class`, `def`, `if`)



 *Learn more in the* [Python Docs – Variables](https://docs.python.org/3/reference/datamodel.html#objects-values-and-types)

Let me know if you’d like a visual example, code sandbox, or interactive notebook!

In python, variables are used to store the data that can be referenced
 What is a variable ?

A Variable in python is like a container used to store data you can assign values using = operator

PYTHON

 name = "Arun"
 age = 20
 is_student = True




#  Python Data Types

Python is a dynamically typed language, which means you don't need to declare a variable's type explicitly. Python has several built-in data types categorized into different classes.



##  Basic Built-in Data Types

###  Numeric Types

| Type      | Description                       | Example      |
| --------- | --------------------------------- | ------------ |
| `int`     | Integer numbers                   | `x = 42`     |
| `float`   | Floating point numbers (decimals) | `pi = 3.14`  |
| `complex` | Complex numbers                   | `z = 2 + 3j` |



###  Text Type

| Type  | Description     | Example          |
| ----- | --------------- | ---------------- |
| `str` | Unicode strings | `name = "Alice"` |



###  Boolean Type

| Type   | Description          | Example           |
| ------ | -------------------- | ----------------- |
| `bool` | True or False values | `is_valid = True` |



##  Collection Data Types

###  List

* Ordered, mutable, allows duplicates.

python
fruits = ["apple", "banana", "cherry"]


###  Tuple

* Ordered, immutable, allows duplicates.

python
dimensions = (1920, 1080)


###  Set

* Unordered, no duplicates.

python
colors = {"red", "green", "blue"}


###  Dictionary

* Key-value pairs, unordered (Python 3.6+ preserves order).

python
person = {"name": "Alice", "age": 30}




##  Other Common Types

| Type        | Description                       | Example              |
| ----------- | --------------------------------- | -------------------- |
| `NoneType`  | Represents the absence of a value | `result = None`      |
| `bytes`     | Immutable byte sequences          | `data = b"hello"`    |
| `bytearray` | Mutable byte sequences            | `arr = bytearray(5)` |
| `range`     | Represents a range of numbers     | `range(0, 10)`       |



##  Type Checking

Use the built-in `type()` and `isinstance()` functions:

python
type(42)              # <class 'int'>
isinstance(42, int)   # True




##  Type Hints (Python 3.5+)

Optional type hints using the `typing` module:

python
def greet(name: str) -> str:
return f"Hello, {name}"




##  Summary Table

| Category | Types                              |
| -------- | ---------------------------------- |
| Numeric  | `int`, `float`, `complex`          |
| Text     | `str`                              |
| Sequence | `list`, `tuple`, `range`           |
| Set      | `set`, `frozenset`                 |
| Mapping  | `dict`                             |
| Boolean  | `bool`                             |
| Binary   | `bytes`, `bytearray`, `memoryview` |
| Special  | `NoneType`                         |



##  References

* [Python Official Docs - Data Types](https://docs.python.org/3/library/stdtypes.html)
* [PEP 484 - Type Hints](https://peps.python.org/pep-0484/)





# Python Variable Naming Rules

In Python, variables are used to store data. Naming variables properly is essential for readable and maintainable code.


##  Rules for Naming Variables

## Valid Variable Names

* Must start with a **letter** (`A–Z`, `a–z`) or an **underscore** (`_`)
* Can contain letters, digits (`0–9`), and underscores (`_`)
* **Case-sensitive** (`name`, `Name`, and `NAME` are different variables)
* **Cannot be a Python keyword**

python
# Valid examples
name = "Arun"
_age = 20
user_1 = "admin"
pi_value = 3.1415



## Invalid Variable Names

python
2cool = "nope"        # ❌ Starts with a digit
first-name = "John"   # ❌ Hyphen not allowed
class = "Physics"     # ❌ 'class' is a reserved keyword


##  Best Practices (PEP 8 Style Guide)

* Use **lowercase letters** and **underscores** for variable names:

  python
  user_name = "arun"
  total_amount = 100.0
  

* Use **UPPER\_CASE** for constants:

  python
  MAX_RETRIES = 5
  

* Avoid using:

  * Single characters like `l`, `O`, or `I` (easily confused with numbers)
  * Ambiguous names like `data1`, `data2`, etc.



## Reserved Keywords (Don’t Use as Variable Names)

These are built-in and have special meaning in Python:


  ( False, None, True, and, as, assert, break, class, continue, def, del,
elif, else, except, finally, for, from, global, if, import, in, is,
lambda, nonlocal, not, or, pass, raise, return, try, while, with, yield )


You can get the full list programmatically:

python
import keyword
print(keyword.kwlist)


## Quick Check

| Variable Name | Valid? | Reason                 |
| ------------- | ------ | ---------------------- |
| `_user`       | ✅     | Starts with underscore |
| `user_123`    | ✅     | Alphanumeric + `_`     |
| `123user`     | ❌     | Starts with digit      |
| `user-name`   | ❌     | Hyphen not allowed     |
| `def`         | ❌     | Python keyword         |



##  References

* [PEP 8 - Python Style Guide](https://peps.python.org/pep-0008/#naming-conventions)
* [Python Keywords (Official Docs)](https://docs.python.org/3/reference/lexical_analysis.html#keywords)





##  Declaring Variables in Python

In Python, variables are used to store data values. You **do not need to declare the data type** explicitly—Python automatically detects the type based on the value assigned.

##  Syntax

python
variable_name = value


* `variable_name`: the name you give to the variable.
* `=`: the assignment operator.
* `value`: the data you want to store.

## Example

python
# Integer
age = 25

# String
name = "Arun"

# Float
price = 19.99

# Boolean
is_active = True


## Variable Naming Rules

* Must start with a **letter** or **underscore** (`_`)
* Can contain **letters**, **numbers**, and **underscores**
* **Case-sensitive** (`name` and `Name` are different)
* **Should not use reserved keywords** (like `class`, `if`, `for`)

## Example with Type Check

python
x = 10
print(type(x))  # <class 'int'>

x = "Python"
print(type(x))  # <class 'str'>


## Best Practices

* Use **meaningful names** (`user_name` instead of `x`)
* Use **snake\_case** for variable names (e.g., `total_amount`)
* Use **lowercase letters** (constants can be in UPPERCASE)


##  Creating Variables in Python


## Example: Creating Different Types of Variables

python
# Integer variable
age = 20

# Float variable
height = 5.9

# String variable
name = "Arun"

# Boolean variable
is_student = True

# List variable
hobbies = ["reading", "coding", "gaming"]

# Dictionary variable
user = {
    "name": "Arun",
    "age": 21,
    "is_student": True
}

# Print all variables
print(name, age, height, is_student)
print("Hobbies:", hobbies)
print("User Info:", user)


## Output:

Arun 21 5.9 True
Hobbies: ['reading', 'coding', 'gaming']
User Info: {'name': 'Arun', 'age': 21, 'is_student': True}

## Quick Notes

* No need to use `var`, `int`, `string`, etc.
* Use descriptive names (`name`, `hobbies`) instead of `x`, `a1`.
* Python uses dynamic typing — you can change the type later.


---

##  Printing Variable Values in Python

Use the `print()` function to display variable values in the console.

## Example

python
name = "Arun"
age = 21

# Print individual variables
print(name)
print(age)

# Print with custom message
print("Name:", name)
print("Age:", age)

# Using f-string (Python 3.6+)
print(f"My name is {name} and I am {age} years old.")


## Output

Arun
21
Name: Arun
Age: 21
My name is Arun and I am 21 years old. 


---


---

## Python Data Types – Quick Overview 

Python has several **built-in data types** used to store values of different kinds:

## Basic Data Types:

| Type      | Example          | Description                | 
| --------- | ---------------- | -------------------------- | 
| `int`     | `x = 10`         | Integer numbers            |
| `float`   | `y = 3.14`       | Decimal numbers            | 
| `complex` | `z = 2 + 3j`     | Complex numbers            | 
| `bool`    | `flag = True`    | Boolean (`True` / `False`) |
| `str`     | `name = "Alice"` | Text or string values      |

## Collection Data Types: 

| Type    | Example                        | Description                   |
| ------- | ------------------------------ | ----------------------------- |
| `list`  | `fruits = ["apple", "banana"]` | Ordered, mutable collection   |
| `tuple` | `coords = (10, 20)`            | Ordered, immutable collection |
| `set`   | `ids = {1, 2, 3}`              | Unordered, unique values      |
| `dict`  | `person = {"name": "Bob"}`     | Key-value pairs               |

## Type Checking

python
print(type(10))        # <class 'int'>
print(type("hello"))   # <class 'str'>


## Type Conversion

python
int("5")     # → 5
str(10)      # → "10" 
list("abc")  # → ['a', 'b', 'c'] 

---
    
Sure! Here's a **short and GitHub-friendly** explanation of the **comma operator in Python**:

---

## Comma in Python – Not an Operator!

In Python, the **comma (`,`) is *not* an operator** like in C/C++.
Instead, it's used to **create tuples** or **separate values** in function arguments, assignments, and loops.

---

## Usage Examples:

python
# Tuple creation
a = 1, 2, 3
print(type(a))  # <class 'tuple'>

# Multiple assignment
x, y = 10, 20

# Function arguments
def add(a, b):
    return a + b

result = add(5, 7)

# Loop with multiple variables
for i, val in enumerate(['a', 'b']):
    print(i, val)


---

## Summary:

* **Comma is a separator**, not an operator.
* Often used to **create tuples** or **unpack variables**.

---

---

## Printing Text Using Comma in Python

In Python, commas inside `print()` **separate multiple values** and insert a **space** between them.

---

### ✅ Example:

python
# Printing multiple values using comma
name = "Arun"
age = 25

print("Name:", name, "| Age:", age)


**Output:**


Name: Arun | Age: 25


---

## Notes:

* Commas let you print different types (like strings + numbers) without converting them.
* Adds automatic spaces between items.

---

---

## Printing with `sep` and `end` in Python

Python’s print() function has two useful optional parameters:

* **`sep`**: Defines the **separator** between multiple items.
* **`end`**: Defines what to print at the **end** of the output (default is a newline `\n`).

---

## `sep` – Separator Between Values

By default, print() separates multiple arguments with a space.

python
print("Python", "is", "awesome")  
# Output: Python is awesome


You can change the separator using `sep`:

python
print("Python", "is", "awesome", sep="-")
# Output: Python-is-awesome


---

## `end` – What to Print at the End

By default, `print()` ends with a newline (`\n`):

python
print("Hello")
print("World")
# Output:
# Hello
# World


You can change this using `end`:

python
print("Hello", end=" ")
print("World")
# Output: Hello World

---

## Combine `sep` and `end`

python
print("2025", "07", "04", sep="-", end="!\n")
# Output: 2025-07-04!

---

## Tip

Use `sep` and `end` to format output **without string concatenation**!

---

## Example: Using `sep` in `print()` (Short Version)

python
print("Hello", "World", "2025", sep=" - ")


**Output:**

Hello - World - 2025

The `sep` parameter sets the **separator** between printed values.

## Example: Using `end` Parameter in `print()`

python
print("Hello", end=" ")
print("World!")

**Output:**

Hello World!

 `end=" "` keeps the cursor on the same line with a space instead of a newline.

---

## Printing with **f-Strings** in Python

**f-Strings** (formatted string literals) make it easy to include variables and expressions inside strings using `{}`.
Available from **Python 3.6+**.

---

## Basic Syntax

python
name = "Arun"
print(f"Hello, {name}!")

**Output:**


Hello, Arun!


 Just add an `f` before the opening quote, and put variables or expressions inside `{}`.

---

## With Expressions

python
a = 5
b = 10
print(f"The sum of {a} and {b} is {a + b}")

**Output:**


The sum of 5 and 10 is 15

---

## Formatting Numbers

python
pi = 3.14159
print(f"Value of pi: {pi:.2f}")

**Output:**


Value of pi: 3.14

---

## Example with Date

python
from datetime import datetime
today = datetime.now()
print(f"Today's date: {today:%Y-%m-%d}")

**Output:**

Today's date: 2025-07-04

---

## Clean & Readable

f-Strings are:

* Faster and more readable than `format()` or `%` formatting
* Great for inline calculations and formatting

---

## Short Example: Using `f-string` in Python

python
name = "Arun"
print(f"Hello, {name}!")

**Output:**

Hello, Arun!

🔹 f-strings let you insert variables directly into strings using `{}`.

## Rounding to Two Decimal Places in Python (Shortly)

Use the built-in `round()` function:

python
num = 3.14159
rounded = round(num, 2)
print(rounded)

**Output:**

3.14

 round(number, 2) rounds the number to 2 decimal places.

---

## Comments in Python

**Comments** are notes in your code to explain what it does. They are **ignored by the Python interpreter**.

---

## Single-Line Comments

Use the `#` symbol:

python
# This is a single-line comment
print("Hello, World!")  # This prints a message

---

## Multi-Line Comments (Workaround)

Python doesn’t have official multi-line comment syntax, but you can use multiple `#`:

python
# This is a comment
# that spans multiple lines
print("Done")

Or use a **docstring** (not recommended unless for documentation):

python
"""
This is a multi-line string
which can act like a comment
"""

>  Note: Triple-quoted strings are not true comments — they are stored as string objects if not assigned.

---

## Best Practices

* Use comments to explain **why**, not **what** (if code is self-explanatory)
* Keep them **short and clear**
* Update comments when code changes

---

## Why Are Comments Used in Python? 

**Comments** are used to:

* Explain code for better readability
* Make the code easier to understand and maintain
* Help other developers (and your future self) know **why** something was done
* Temporarily disable code during debugging

 Comments are ignored by the Python interpreter.

##  Example: Comments in Python

python
# This prints a welcome message
print("Welcome to Python!")

🔹 The `#` makes everything after it a comment (ignored by Python).

---

## Printing a String Multiple Times in Python

Use the `*` operator to repeat a string:

python
print("Hello " * 3)

**Output:**

Hello Hello Hello 

 The `*` operator repeats the string **n** times.

---

## Example: Multi-line String in Python

You can use triple quotes (`'''` or `"""`) to create a multi-line string:

python
message = """Hello,
This is a multi-line
string in Python."""
print(message)

**Output:**

Hello,
This is a multi-line
string in Python.

🔹 Triple quotes preserve line breaks and spacing.

---

## Type Casting in Python

**Type casting** means converting a value from one data type to another (e.g., `int` to `float`, `str` to `int`, etc.).

Python provides built-in functions for casting:

---

## Common Type Casting Functions

| Function  | Converts to... |
| --------- | -------------- |
| `int()`   | Integer        |
| `float()` | Floating point |
| `str()`   | String         |
| `bool()`  | Boolean        |

---

## Examples

python
# String to int
num = int("10")         # 10

# Float to int (truncates)
x = int(3.7)            # 3

# Int to float
y = float(5)            # 5.0

# Number to string
text = str(123)         # "123"

# Non-zero to True
val = bool(1)           # True

---

## Note

Type casting may raise errors if the conversion is invalid:

python
int("abc")  #  ValueError

---

## Use Cases

* Accepting user input (`input()` returns a string)
* Mathematical operations
* Data processing and validation

---

---

## Example: A  ( Calculating Total Salary in Python )

## **Theory**

To calculate total salary, you typically use:

total_salary = basic_salary + allowances - deductions

Where:

* **basic\_salary**: Fixed base salary
* **allowances**: Extra income (e.g., HRA, travel, etc.)
* **deductions**: Amounts subtracted (e.g., tax, PF, etc.)

You can use variables and simple arithmetic to compute this.

---

## **Python Code Example**

python
# Define salary components
basic_salary = 25000
allowances = 5000
deductions = 3000

# Calculate total salary
total_salary = basic_salary + allowances - deductions

# Display the result
print(f"Total Salary: ₹{total_salary}")

---

### 📌 Output:

Total Salary: ₹27000

---

## Tip

You can also use `input()` to take user input for dynamic salary calculation:

python
basic = float(input("Enter basic salary: "))
allow = float(input("Enter allowances: "))
deduct = float(input("Enter deductions: "))

total = basic + allow - deduct
print(f"Total Salary: ₹{total}")

---

Example: B  coverting string to float

The following code converts Ivan's salary from a string to float;otherwise, the program generates an error.
Arun's wage is not enclosed with a double quote;therefore, it is already a number and doesn't need to be covrerted

calculator.py

salary_ivan=3200
salary_Arun="2800"
total_salary=salary_ivan+float(salary_Arun)
print("Total salaries:$",total_salary)

OUTPUT

Total salaries:$6000.0

---
Example: C  coverting string to Int

To calculate the age difference between two individuals, you must covert the second age to int type because the second age is a string
      
calculate.py 

age1=22
age2"34"
age_difference=int(age2)-age1
print("Age Difference:",age_difference)

OUTPUT

Age Difference: 12

---
   
---

## Escape Sequences in Python

**Escape sequences** are special characters used in strings to represent characters that are otherwise difficult to include directly, like newlines, tabs, quotes, etc.

They begin with a **backslash (`\`)**.

---

## Common Escape Sequences:

| Escape | Meaning          | Example Output                |
| ------ | ---------------- | ----------------------------- |
| `\n`   | New line         | Splits the text to a new line |
| `\t`   | Tab (horizontal) | Adds a tab space              |
| `\\`   | Backslash        | Prints `\` character          |
| `\'`   | Single quote     | Prints `'` in a string        |
| `\"`   | Double quote     | Prints `"` in a string        |

---

## Example:

python
# Using escape sequences
print("Hello\nWorld")     # New line
print("Python\tRocks")    # Tab space
print("He said: \"Yes\"") # Double quotes inside string
print('It\'s awesome!')   # Single quote inside string

---

## Output:


Hello
World
Python	Rocks
He said: "Yes"
It's awesome!

---

## Tip:

You can also use **raw strings** (`r"..."`) to **ignore escape sequences**.

python
print(r"This is a raw string:\nNo new line here.")

🧾 Output:

This is a raw string:\nNo new line here.

---

---

## Escape Sequence Quiz (Python)

Test your knowledge of escape sequences!
**Choose the correct output or fill in the blanks.**

---

## 1. What will this code print?

python
print("Hello\nPython")


A. Hello Python
B. Hello\nPython
C. Hello
        Python
D. Error

> ✅ **Answer:** C

---

## 2. Which escape sequence is used to insert a tab space?

A. \\n
B. \t
C. \n
D. \b

> ✅ **Answer:** B

---

 QUIZ: 2
 
## 1. Fill in the blank to print this output:

He said: "Hello"

python
print("He said: _______")

> ✅ **Answer:** "He said: \"Hello\""

---

## 2. What is the output of this code?

python
print('It\'s easy!')


A. It's easy!
B. Its easy!
C. It\'s easy!
D. Error

> ✅ **Answer:** A

---

---

## Escape Sequence Quiz – *Total Weight in a Lift*

**Scenario:**
You're building a Python program to display the **total weight of 3 people** inside a lift.
Use **escape sequences** to format the output nicely.

---

## Task:

Fill in the blanks ( ___ ) to complete the program.

python
# Lift Weight Calculator

person1 = 65.5
person2 = 72.0
person3 = 58.3

# Calculate total weight
total_weight = person1 + person2 + person3

# Print the result using escape sequences
print("Lift Weight Report\n")
print("Person 1:\t", person1, "kg")
print("Person 2:\t", person2, "kg")
print("Person 3:\t", person3, "kg")
print("\nTotal:\t\t", total_weight, "kg")

---

## Quiz Questions:

1. What does \n do in the print statement?

   * A. Adds a new line
   * B. Adds a tab
   * C. Prints a slash
   * D. None of the above

2. What is the purpose of \t in this code?

   * A. New paragraph
   * B. Adds a tab space for alignment
   * C. Skips the line
   * D. None

3. What is the **total weight** calculated in the program?

---

## Expected Output:

Lift Weight Report

Person 1:	 65.5 kg
Person 2:	 72.0 kg
Person 3:	 58.3 kg

Total:		 195.8 kg

---

---

## Escape Sequence Exercise – *Printing Variable Values & Types*

** Objective:**
Practice using **escape sequences** (`\n`, `\t`) along with `print()`, `type()`, and variables.

---

###  Instructions:

1. Declare 3 different variables with different data types.
2. Use print() to:

   * Show each variable's **value**
   * Show its **type**
   * Use **\n for new lines** and **\t for indentation**
3. Try to format the output to look clean and readable.

---

###  Sample Code (Complete This):

python
# Variable Declarations
name = "Alice"
age = 25
height = 5.4

# Print values and types using escape sequences
print("Variable Info:\n")

print("Name:\t", name)
print("Type:\t", type(name), "\n")

print("Age:\t", age)
print("Type:\t", type(age), "\n")

print("Height:\t", height)
print("Type:\t", type(height), "\n")

---

## Expected Output:

Variable Info:

Name:	 Alice
Type:	 <class 'str'>

Age:	 25
Type:	 <class 'int'>

Height:	 5.4
Type:	 <class 'float'>

---

## Challenge Yourself:

* Try with bool and list types too.
* Use f-strings instead of commas in print() for cleaner formatting.

---

## Exercise: Print a Shape Using Escape Sequences

** Task:**
Use **\n** (new line) and **\t** (tab) escape sequences to print the following triangle shape:

	    *
	   * *
	  * * *
	 * * * *

---

## Starter Code:

python
# Print triangle using escape sequences
print("\t\t\t*")
print("\t\t  * *")
print("\t    * * *")
print("      * * * *")

---

## Instructions:

* Use \t for horizontal spacing (tab).
* Use \n if printing all lines together in a single `print()` statement.
* Try modifying the shape or adding more lines!

---

---

## Python Operators – Quick Guide

**Operators** are special symbols used to perform **operations** on variables and values.

---

## 1. **Arithmetic Operators**

Used for basic math.

| Operator | Description        | Example        |
| -------- | ----------------- | -------------- |
| +      | Addition            | `3 + 2 = 5`    |
| -      | Subtraction         | `5 - 1 = 4`    |
| *      | Multiplication      | `4 * 2 = 8`    |
| /      | Division            | `10 / 2 = 5.0` |
| //     | Floor Division      | `10 // 3 = 3`  |
| %      | Modulus (Remainder) | `10 % 3 = 1`   |
| **     | Exponentiation      | `2 ** 3 = 8`   |

---

## 2. **Comparison Operators**

Compare two values and return `True` or `False`.

| Operator | Description      | Example         |
| -------- | ---------------- | --------------- |
| `==`     | Equal to         | `5 == 5 → True` |
| `!=`     | Not equal to     | `3 != 4 → True` |
| `>`      | Greater than     | `7 > 2 → True`  |
| `<`      | Less than        | `2 < 5 → True`  |
| `>=`     | Greater or equal | `5 >= 5 → True` |
| `<=`     | Less or equal    | `4 <= 6 → True` |

---

### 🔹 3. **Assignment Operators**

Used to assign values.

| Operator | Meaning             | Example              |
| -------- | ------------------- | -------------------- |
| `=`      | Assign              | `x = 10`             |
| `+=`     | Add and assign      | `x += 5 → x = x + 5` |
| `-=`     | Subtract and assign | `x -= 3 → x = x - 3` |
| `*=`     | Multiply and assign | `x *= 2`             |
| `/=`     | Divide and assign   | `x /= 4`             |

---

### 🔹 4. **Logical Operators**

Used to combine conditions.

| Operator | Description           | Example            |
| -------- | --------------------- | ------------------ |
| `and`    | True if both are true | `x > 5 and x < 10` |
| `or`     | True if one is true   | `x < 3 or x > 8`   |
| `not`    | Reverses the result   | `not(x == 5)`      |

---

### 🔹 5. **Identity Operators**

Used to compare object identity.

| Operator | Meaning             | Example      |
| -------- | ------------------- | ------------ |
| `is`     | True if same object | `x is y`     |
| `is not` | True if not same    | `x is not y` |

---

### 🔹 6. **Membership Operators**

Check if a value exists in a sequence.

| Operator | Meaning              | Example              |
| -------- | -------------------- | -------------------- |
| `in`     | Value exists         | `"a" in "apple"`     |
| `not in` | Value does not exist | `"z" not in "apple"` |

---

## Example Code:

python
x = 10
y = 5

print(x + y)       # Arithmetic
print(x > y)       # Comparison
print(x == 10 and y == 5)  # Logical
x += 2             # Assignment
print(x)

---

# Example for Arithmetic Operators in Python

a = 10
b = 3

# Addition
print("Addition:", a + b)

# Subtraction
print("Subtraction:", a - b)

# Multiplication
print("Multiplication:", a * b)

# Division
print("Division:", a / b)

# Floor Division
print("Floor Division:", a // b)

# Modulus
print("Modulus:", a % b)

# Exponentiation
print("Exponentiation:", a ** b)

## Modulus (`%`) in Python – Short Explanation

The **modulus operator %** returns the **remainder** of a division.

#### Example:

python
print(10 % 3)  # Output: 1

 Here, 10 ÷ 3 = 3 with a **remainder of 1** → so 10 % 3 gives 1.

## Use Cases:

* Check if a number is even/odd:

  python
  print(7 % 2)  # Output: 1 → odd
  print(8 % 2)  # Output: 0 → even
  
* Looping in cycles, e.g., `i % 4` cycles 0,1,2,3,0,...
* Useful in clock-based logic or round-robin systems.

---

python
# Modulus Example

a = 17
b = 5

result = a % b
print("Remainder:", result)  # Output: 2

 **Explanation:** 17 ÷ 5 = 3 remainder **2**, so 17 % 5 = 2.

---

## Floor Division in Python (`//`) 

**Floor division** returns the **quotient** of a division, **rounded down** to the nearest whole number.

## Syntax:

python
a // b

## Example:

---

# Floor Division Example

a = 17
b = 5

result = a // b
print("Quotient:", result)  # Output: 3

 **Explanation:**
17 ÷ 5 = 3.4 → floor division 17 // 5 = 3 (rounds down).

Common use: Get whole number part of a division without decimals.

---
    
## Assignment Operator in Python — Short & GitHub-Friendly

The **assignment operator `=`** is used to **assign a value** to a variable.

## Example:

# Assignment Operator Example

x = 10  # Assigns 10 to variable x
print("x =", x)


## Other compound assignment operators:

python
x += 5   # x = x + 5
x -= 2   # x = x - 2
x *= 3   # x = x * 3
x /= 2   # x = x / 2

 **Tip:** Assignment operators help update variable values concisely.
    
---

# Assignment Operator Example

x = 5
print("x =", x)  # Output: x = 5

 This assigns the value 5 to the variable x.

---

##  Using `+` and `+=` with Strings in Python 

####  `+` Operator → **Concatenates** strings (joins them)

greeting = "Hello, " + "World!"
print(greeting)  # Output: Hello, World!

## `+=` Operator → **Appends** to an existing string

message = "Hello"
message += ", Python!"
print(message)  # Output: Hello, Python!

 **Tip:**

* + creates a **new string**
* += updates the **existing string variable**

 Useful for building strings in loops or step-by-step.

---
Example for concatenate strings using "+"

# String Concatenation using +

first = "Hello"
second = "World"
result = first + " " + second
print(result)  # Output: Hello World

---

 Here's a short example for **concatenating strings using `+=`**:

# String Concatenation using +=

text = "Hello"
text += " World"
print(text)  # Output: Hello World

 += adds " World" to the existing text string.

---

## Comparison Operators in Python 

**Comparison operators** are used to **compare values**. They return either True or False.

## List of Comparison Operators:

| Operator | Meaning               | Example           |
| -------- | --------------------- | ----------------- |
| `==`     | Equal to              | `5 == 5` → `True` |
| `!=`     | Not equal to          | `5 != 3` → `True` |
| `>`      | Greater than          | `7 > 2` → `True`  |
| `<`      | Less than             | `3 < 4` → `True`  |
| `>=`     | Greater than or equal | `5 >= 5` → `True` |
| `<=`     | Less than or equal    | `2 <= 3` → `True` |

## Example:

a = 10
b = 5

print(a > b)   # True
print(a == b)  # False

 **Tip:** Commonly used in `if` statements, loops, and filters.

---

 A short example for **comparison operators** in Python:


# Comparison Operator Example

a = 7
b = 5

print(a > b)   # True
print(a == b)  # False

 Compares values and returns True or False.

---

## Logical Operators in Python 

**Logical operators** are used to combine conditional statements. They return True or False.

## Types of Logical Operators:

| Operator | Description                      | Example                    |
| -------- | -------------------------------- | -------------------------- |
| `and`    | True if **both** are True        | `True and False` → `False` |
| `or`     | True if **at least one** is True | `True or False` → `True`   |
| `not`    | Reverses the result              | `not True` → `False`       |

## Example:

python
a = 5
b = 10

print(a > 2 and b > 8)   # True
print(a < 3 or b == 10)  # True
print(not(a == b))       # True


**Tip:** Used in if statements to combine multiple conditions.

---

  A short example for **logical operators** in Python:

python
# Logical Operator Example

x = 10
y = 5

print(x > 5 and y < 10)   # True
print(x < 5 or y == 5)    # True
print(not(x == y))        # True

 Combines conditions using and, or, not.

---

## Identity Operators in Python 

**Identity operators** are used to **compare the memory location** of two objects.

## Types of Identity Operators:

| Operator | Description                                      | Example      |
| -------- | ------------------------------------------------ | ------------ |
| `is`     | Returns `True` if **both refer to same object**  | `a is b`     |
| `is not` | Returns `True` if **they are different objects** | `a is not b` |

## Example:

a = [1, 2, 3]
b = a
c = [1, 2, 3]

print(a is b)      # True  (same object)
print(a is c)      # False (different object with same value)
print(a is not c)  # True

 **Note:** Use == to compare **values**, is to compare **identity**.

---

A short example for **identity operators** in Python:

# Identity Operator Example

a = [1, 2]
b = a
c = [1, 2]

print(a is b)      # True
print(a is c)      # False
print(a is not c)  # True

 `is` checks if both refer to the **same object in memory**.

---

## Membership Operators in Python 

**Membership operators** are used to **check if a value exists** in a sequence (like a list, string, tuple, etc).

## Types of Membership Operators:

| Operator | Description                                | Example                       |
| -------- | ------------------------------------------ | ----------------------------- |
| `in`     | Returns `True` if value is present         | `"a" in "apple"` → `True`     |
| `not in` | Returns `True` if value is **not** present | `3 not in [1, 2, 4]` → `True` |

## Example:

fruits = ["apple", "banana", "cherry"]

print("apple" in fruits)     # True
print("grape" not in fruits) # True

 **Tip:** Great for searching in strings, lists, and other collections.

 ---

 A short quiz on **arithmetic operators**:

---

## **Quiz:**

What will be the output of the following code?

x = 8
y = 3
print(x % y + x // y)

**A.** 3
**B.** 5
**C.** 4
**D.** 6

---

 A short quiz on the **assignment operator**:

---

## **Quiz: Assignment Operator**

**Question:**
What will be the output of the following code?

x = 10
x += 5
print(x)

**A.** 10
**B.** 5
**C.** 15
**D.** Error

---

 **Answer:** C. 15
**Explanation:** `x += 5` means `x = x + 5`, so `10 + 5 = 15`.

--- 

Sure! Here's a short quiz for comparison operators in Python:

---

** Quiz: Comparison Operator in Python**

**Question:**
What will be the output of the following code?

x = 10
y = 20
print(x > y)

**A.** True
**B.** False
**C.** 10
**D.** 20

---

*Correct Answer:* **B. False**
**Explanation:** `10 > 20` is not true, so it returns `False`.

---


## **Quiz: Identity Operator in Python**

**Question:**
What will be the output of the following code?

x = [1, 2, 3]
y = x
z = [1, 2, 3]

print(x is y)
print(x is z)

**Options:**
A) `True` `True`
B) `True` `False`
C) `False` `True`
D) `False` `False`

---

**Answer:**  **B) True False**

**Explanation:**

* `x is y` → `True` because `y` refers to the same object as `x`.
* `x is z` → `False` because `z` is a new list with the same values, but it's a different object in memory.

---

##  User Input & Strings in Python

## Getting User Input

Python uses the input() function to get data from the user.

name = input("Enter your name: ")
print("Hello,", name)

* input() always returns data as a **string**.

## Working with Strings

You can use **string methods** to manipulate text:

text = "  python is FUN!  "

print(text.strip())       # Removes leading/trailing spaces
print(text.lower())       # Converts to lowercase
print(text.upper())       # Converts to uppercase
print(text.replace("FUN", "awesome"))  # Replaces words

## Concatenating Strings

Join strings using `+` or `f-strings`:

first = "Hello"
last = "World"

print(first + " " + last)        # Using +
print(f"{first} {last}!")        # Using f-string

---

 **Tip:** Always convert input to the needed type (e.g., `int(input())` for numbers).

---

## **User Input in Python (Short)**

Python uses the `input()` function to take input from the user.

name = input("Enter your name: ")
print("Hello,", name)

* input() **always returns a string**.
* You can convert input to other types using `int()`, `float()`, etc.

age = int(input("Enter your age: "))
print("You will be", age + 1, "next year.")

---

Example: To create a triangle using user input:

rows = int(input("Enter number of rows: "))

for i in range(1, rows + 1):
    print("*" * i)

## Sample Output:

If user enters `5`:

*
**
***
****
*****

This prints a **right-angled triangle** of stars (`*`).

Example: to calculate **total weight** using user input:

item1 = float(input("Enter weight of item 1 (kg): "))
item2 = float(input("Enter weight of item 2 (kg): "))
total = item1 + item2

print("Total weight:", total, "kg")

## Sample Output:

Enter weight of item 1 (kg): 2.5  
Enter weight of item 2 (kg): 3.2  
Total weight: 5.7 kg

Example: to check the **variable types** using `type()` in Python:

name = "Alice"
age = 25
height = 5.6
is_student = True

print(type(name))      # <class 'str'>
print(type(age))       # <class 'int'>
print(type(height))    # <class 'float'>
print(type(is_student))# <class 'bool'>

## Output:

<class 'str'>
<class 'int'>
<class 'float'>
<class 'bool'>

---

Example for converting strings to integers using user input:

# Get user input
num = input("Enter a number: ")

# Convert string to integer
num = int(num)

# Display result
print("You entered:", num)

 **Note:** `input()` always returns a string. Use `int()` to convert it to an integer.

---

explanation of **strings and substrings** in Python:

---

## Strings in Python

* A **string** is a sequence of characters enclosed in quotes (' ' or " ").
* Example:

  message = "Hello, Python!"
  
## Substrings

* A **substring** is a part of a string.

* You can extract substrings using **slicing**:

  text = "Programming"
  print(text[0:6])  # Output: Progra
  
* You can also **check** if a substring exists:

  "gram" in text   # True
  
---

**Tip:** Python strings are **zero-indexed**.

 **Test it out**:

word = "education"
print(word[1:4])         # duc
print("cat" in word)     # True

---

 Explanation of **string indexing** in Python:

---

## String Index in Python

* **Indexing** lets you access individual characters in a string.
* Index starts at **0** (zero-based indexing).

text = "Python"
print(text[0])  # P
print(text[5])  # n

* You can also use **negative indexes** to count from the end:

print(text[-1])  # n (last character)
print(text[-3])  # h

---

 **Tip:** Use indexes to loop, slice, or manipulate characters in strings.

A short example for **string index**:

name = "Python"
print(name[0])   # Output: P
print(name[3])   # Output: h
print(name[-1])  # Output: n (last character)

 This shows how to access characters using positive and negative indexes.

  A explanation of **substrings** in Python:

---

## Substrings in Python

* A **substring** is a part of a string.

* Use **slicing** to get substrings:

  text = "HelloWorld"
  print(text[0:5])  # Output: Hello
  
* Check if a substring exists:

  print("World" in text)  # True

---

 **Syntax:** string[start:end]
(start index is included, end index is excluded)

 **Try this:**

word = "education"
print(word[2:5])       # uca
print("cat" in word)   # True

---

 explanation of using **operators with strings** in Python:

---

## Using Operators with Strings

Python allows some operators to work with strings:

## `+` (Concatenation)

* Joins two strings:

  first = "Hello"
  second = "World"
  result = first + " " + second
  print(result)  # Output: Hello World
  
## `*` (Repetition)

* Repeats a string multiple times:

  text = "Hi "
  print(text * 3)  # Output: Hi Hi Hi 

## Comparison Operators

* Strings can be compared using `==`, `!=`, `<`, `>`, etc.

  print("apple" == "apple")  # True
  print("a" < "b")           # True
  
---

 **Tip:** Use `+` to build strings, and `*` to repeat patterns.

---

short example for **comparing strings**:

a = "apple"
b = "banana"

print(a == b)   # False
print(a < b)    # True (because "apple" comes before "banana")

 You can use `==`, `!=`, `<`, `>`, `<=`, `>=` to compare strings alphabetically.


