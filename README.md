
# 🧠 AI Lab Series – PyTorch & Machine Learning

This repository supports a hands-on AI lab series following the completion of:
- Linear Algebra
- Calculus
- Statistics

The goal is to transition from **math foundations → real AI implementation using PyTorch**.

Each class is 60 minutes and structured for middle/high school students with limited programming experience.

---

# 📅 Course Overview

| Class | Topic | Focus |
|-------|-------|-------|
| 1 | Python Programming Basics | Learn coding fundamentals + Colab + GitHub |
| 2 | Intro to PyTorch & Math Ops | Tensors and numerical operations |
| 3 | Build First Neural Network | Supervised learning & regression |
| 4 | CNN for Image Recognition | Computer vision & deeper models |
| 5 | Advanced Concepts | Optimization, regularization, GPU, and future directions |

---

# 🧩 Class 1 – Programming with Python (60 min)

## 🎯 Goal
Students with zero coding background learn:
- Python basics
- How to run notebooks in Google Colab
- Basic GitHub usage

## ⏱ Structure

### 0–10 min: Why Programming Matters
- Code = instructions for math
- AI models are just programmable math functions

### 10–30 min: Python Basics

```python
print("Hello AI")
x = 5
y = 3
z = x + y
print(z)
```

Topics:
- Variables
- Data types (int, float, string, list)
- Loops
- Functions

### 30–45 min: Using Google Colab
- Run cells
- Add markdown
- Restart runtime
- Install packages

### 45–55 min: Intro to GitHub
- What is version control?
- Clone repository
- Commit & push
- Why professionals use GitHub

### 55–60 min: Quick Challenge
- Write a function that squares a number.

---

# 🔢 Class 2 – Intro to PyTorch & Math Operations (60 min)

## 🎯 Goal
Understand tensors and math operations in PyTorch.

## 0–15 min: What is PyTorch?
- Open-source ML framework
- Built on tensors
- Dynamic computation graph
- Compare with TensorFlow (more flexible, pythonic)

## 15–45 min: Tensor Math

```python
import torch

a = torch.tensor([1,2,3])
b = torch.tensor([4,5,6])

print(a + b)
print(a - b)
print(a * b)
print(a / b)
print(a % b)
print(a ** 2)
```

Topics:
- Addition
- Subtraction
- Multiplication
- Division
- Remainder (%)
- Exponents (**)
- In-place operations (+=, -=)

Explain tensor shapes and broadcasting.

## 45–60 min: Mini Exercises
- Create random tensor
- Compute mean
- Matrix multiplication

---

# 🤖 Class 3 – Build a Simple Neural Network (60 min)

## 🎯 Goal
Build and train a regression model.

## 0–15 min: What is a Neural Network?
- Layers
- Weights
- Activation functions
- Supervised vs Unsupervised

## 15–45 min: Build Model

```python
import torch
import torch.nn as nn

model = nn.Sequential(
    nn.Linear(1, 10),
    nn.ReLU(),
    nn.Linear(10, 1)
)
```

Loss function:

```python
loss_fn = nn.MSELoss()
```

Optimizer:

```python
optimizer = torch.optim.SGD(model.parameters(), lr=0.01)
```

Training loop explained step by step.

## 45–60 min: Visualize Results
- Plot predictions vs true values
- Discuss overfitting

---

# 🖼 Class 4 – CNN for Image Recognition (60 min)

## 🎯 Goal
Build simple CNN for MNIST.

## 0–15 min: What is a CNN?
- Convolution
- Filters
- Feature maps
- Pooling

## 15–45 min: Build CNN

```python
import torch.nn as nn
import torch

class SimpleCNN(nn.Module):
    def __init__(self):
        super().__init__()
        self.conv1 = nn.Conv2d(1, 16, 3)
        self.pool = nn.MaxPool2d(2,2)
        self.fc1 = nn.Linear(16*13*13, 10)

    def forward(self, x):
        x = self.pool(torch.relu(self.conv1(x)))
        x = x.view(x.size(0), -1)
        x = self.fc1(x)
        return x
```

Explain:
- Feature extraction
- Why CNN works for images

## 45–60 min: Train & Evaluate
- Accuracy
- Confusion matrix
- What happens when model improves?

---

# 🚀 Class 5 – Advanced Concepts (60 min)

## 🎯 Goal
Expose students to deeper AI ideas.

Possible topics:

### Optimization
- SGD vs Adam
- Learning rate

### Regularization
- Dropout
- Weight decay

### GPU Acceleration

```python
device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
print(device)
```

### Ethics & AI Safety
- Bias
- Data privacy
- Responsible AI

### Final Project Idea
- Build small classifier
- Present findings

---

# 🧠 Key Message for Students

Deep learning is:

Linear Algebra + Calculus + Statistics + Code + Data

You already learned the math.  
Now you're learning how to bring it to life.

---

# 📌 Instructor Notes

- Keep coding slow and deliberate.
- Live-code mistakes on purpose.
- Ask prediction questions before running cells.
- Celebrate working code.

---

# 📂 Repository Structure Suggestion

/Class1_Python_Basics.ipynb  
/Class2_Torch_Tensors.ipynb  
/Class3_Regression_Model.ipynb  
/Class4_CNN_MNIST.ipynb  
/Class5_Advanced_Topics.ipynb  
README.md  

---

End of README
