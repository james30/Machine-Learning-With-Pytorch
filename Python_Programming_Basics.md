
# 🧠 AI Lab Series – Python Programming Basics

This repository supports a hands-on AI lab series following the completion of:
- Linear Algebra
- Calculus
- Statistics

The goal is to transition from **math foundations → real AI implementation using PyTorch**.


---

# 📅 Class Overview

| Topic | Focus | 
|-------|-------|
| 1 | Programming Basic |
| 1 | Python Programming With Colab and Github |
| 2 | Variables & Data Types |  
| 3 | Input & Output |  
| 4 | Conditionals & Loops | 
| 5 | Data Structures |  
| 3 | Functions | 
| 4 | Basic Error Handling |  
| 5 |File I/O | 

---

# 🧩 Class 1 – Programming with Python  

## 🎯 Goal
Students with zero coding background learn:
- Python basics
- How to run notebooks in Google Colab
- Basic GitHub usage

## ⏱ Topics

### What Programming Actually Is
- What is a program?  Why and How? Basic Syntax & Running Code
- Code = instructions for math
- AI models are just programmable math functions

### Python Programming With Colab and Github
- Learn coding fundamentals + Colab + GitHub
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
  price = 2.5
  print("A dozen of eggs cost $:", area)
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
- Exercise 1
  ```
  try:
    age = int(input("Enter your age: "))
    print("Next year you will be", age + 1)
  except ValueError:
    print("Please enter a valid number!")
  ```
- Exercise 2
  ```
  try:
    number = int(input("Enter a number: "))
    result = 10 / number
    print("Result:", result)
  except ZeroDivisionError:
    print("You cannot divide by zero!")
  except ValueError:
    print("Please enter a valid number!")
  ```

### File I/O
- Reading from a text file
- Writing to a file

#### Interactive exercises:
- Exercise 1
  ```
  message = input("Write a short note: ")

  # Save it to a file
  with open("note.txt", "w") as file:
      file.write(message)
  
  print("Your note has been saved!")
  ```
- Exercise 2
  ```
  with open("note.txt", "r") as file:
      content = file.read()
  
  print("Here is what you saved:")
  print(content)
  ```
---

End of README
