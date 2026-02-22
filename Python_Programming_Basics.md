
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
| 2 | Python Programming With Colab and Github |
| 3 | Variables & Data Types |  
| 4 | Input & Output |  
| 5 | Conditionals | 
| 6 | Loops
| 7 | Data Structures |  
| 8 | Functions | 
| 9 | Basic Error Handling |  
| 10 | File I/O |
| 11 | Simple Student Gradebook |

---

# 🧩 Class 1 – Programming with Python  

## 🎯 Goal
Students with zero coding background learn:
- Python basics
- How to run notebooks in Google Colab
- Basic GitHub usage

## ⏱ Topics

### Programming Basic
- What is a program? 
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
  print("A dozen of eggs cost $", price)
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

### Conditionals 
- if
- elif
- else
- Comparison operators
- Logical operators (and, or, not)

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

### Loops
- for loops
- while loops
- range()
- Loop control (break, continue)

#### Interactive exercises:
- Exercise 1
  ```
  for i in range(5):
    print(i)
  ```
- Exercise 2
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
### Simple Student Gradebook
Write a Python program that:

- Collects student names and grades
- Stores them in a structured way
- Displays all students
- Calculates basic statistics (average, highest, lowest)

#### Instructions
##### Step 1 — Collect Student Data
- Ask for the student’s name (string)
- Ask for the student’s grade (float)
- Store the data in a list of dictionaries like this:
- {"name": "Alice", "grade": 91}
##### Step 2 — Display All Students

Write a function:

def display_students(students):

This function should print all student names and grades.

##### Step 3 — Compute Statistics

Write three functions:

- def calculate_average(students):
- def find_highest(students):
- def find_lowest(students):

They should:
- Return the average grade
- Return the student with the highest grade

Return the student with the lowest grade

#### Interactive exercises:
- Exercise 1
  ```
  def display_students(students):
    print("\nStudent List:")
    for student in students:
        print(f"{student['name']}: {student['grade']}")


  def calculate_average(students):
      total = 0
      for student in students:
          total += student["grade"]
      return total / len(students)
  
  
  def find_highest(students):
      highest = students[0]
      for student in students:
          if student["grade"] > highest["grade"]:
              highest = student
      return highest
  
  
  def find_lowest(students):
      lowest = students[0]
      for student in students:
          if student["grade"] < lowest["grade"]:
              lowest = student
      return lowest
  
  
  # Main Program
  students = []
  
  num_students = int(input("How many students? "))
  
  for i in range(num_students):
      name = input(f"Enter name of student #{i+1}: ")
      grade = float(input(f"Enter grade for {name}: "))
      
      students.append({
          "name": name,
          "grade": grade
      })
  
  display_students(students)
  
  average = calculate_average(students)
  highest = find_highest(students)
  lowest = find_lowest(students)
  
  print("\nStatistics:")
  print(f"Average grade: {average:.2f}")
  print(f"Highest grade: {highest['name']} ({highest['grade']})")
  print(f"Lowest grade: {lowest['name']} ({lowest['grade']})")
  ```
---

End of README
