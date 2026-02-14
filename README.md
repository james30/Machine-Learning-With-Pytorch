
# 🧠 AI Lab Series – Python Programming Basics

This repository supports a hands-on AI lab series following the completion of:
- Linear Algebra
- Calculus
- Statistics

The goal is to transition from **math foundations → real AI implementation using PyTorch**.


---

# 📅 Class Overview

| Topic | Focus | Focus |
|-------|-------|-------|
| 1 | What Programming Actually Is | What is a program?  Why and How? Basic Syntax & Running Code |
| 1 | Python Programming Basics | Learn coding fundamentals + Colab + GitHub |
| 2 | Variables & Data Types | Variables, Integers, Floats, Strings, Booleans, Type conversion (int(), str()) |
| 3 | Input & Output | Supervised learning & regression |
| 4 | Conditionals & Loops | Computer vision & deeper models |
| 5 | Data Structures | Optimization, regularization, GPU, and future directions |
| 3 | Functions | Supervised learning & regression |
| 4 | Basic Error Handling | Computer vision & deeper models |
| 5 |File I/O | Optimization, regularization, GPU, and future directions |

---

# 🧩 Class 1 – Programming with Python  

## 🎯 Goal
Students with zero coding background learn:
- Python basics
- How to run notebooks in Google Colab
- Basic GitHub usage

## ⏱ Topics

### What Programming Actually Is
- Code = instructions for math
- AI models are just programmable math functions

### Python Programming Basics
- Coding fundamentals
- Colab + GitHub

#### Interactive exercises:
- Exercise 1
  ```
  print("Hello, Python!")
  ```

### Variables & Data Types
- Variables
- Integers
- Floats
- Strings
- Booleans
- Type conversion (int(), str())

#### Interactive exercises:
- Exercise 1
    ```
  length = 5
  width = 3
  area = length * width
  print("The area is:", area)
  ```
- Exercise 2
  ```
  length = 5
  width = 3
  area = length * width
  print("The area is:", area)
  ```

### Input & Output
- input()
- Converting input types
- Basic string formatting (f-strings)

#### Interactive exercises:
- Exercise 1
  ```
  name = input("What is your name? ")
  print("Hello", name)
  ```
- Exercise 2
  ```
  age = int(input("How old are you? "))
  print("In five years you will be", age + 5)
  ```

### Conditionals & Loops
- if
- elif
- else
- Comparison operators
- Logical operators (and, or, not)
- for loops
- while loops
- range()
- Loop control (break, continue)

#### Interactive exercises:
- Exercise 1
  ```
  number = int(input("Enter a number: "))
  if number > 0:
    print("Positive")
  else:
    print("Not positive")
  ```
- Exercise 2
  ```
  score = int(input("Enter your score: "))
  if score >= 90:
    print("A")
  else:
    print("Not A")
  ```
- Exercise 3
  ```
  for i in range(5):
    print(i)
  ```
- Exercise 4
  ```
  for i in range(1, 6):
    print("Number:", i)
  ```

### Data Structures
- Lists
- List indexing
- List methods (append, remove, etc.)
- Basic tuples
- Dictionaries (key-value concept)

#### Interactive exercises:
- Exercise 1
  ```
  fruits = ["apple", "banana", "orange"]
  print(fruits[0])
  ```
- Exercise 2
  ```
  numbers = [1, 2, 3]
  numbers.append(4)
  print(numbers)
  ```

### Functions
- Defining functions
- Parameters
- Return values
- Scope (basic understanding)

#### Interactive exercises:
- Exercise 1
  ```
  def greet(name):
    print("Hello", name)

  greet("Alex")
  ```
- Exercise 2
  ```
  def add(a, b):
    return a + b

  result = add(3, 4)
  print(result)
  ```

### Basic Error Handling
- Common errors (SyntaxError, TypeError)
- Reading tracebacks
- try/except (light intro)

#### Interactive exercises:
- Print Hello World Function

### File I/O
- Reading from a text file
- Writing to a file

#### Interactive exercises:
- Print Hello World Function
  
---

End of README
