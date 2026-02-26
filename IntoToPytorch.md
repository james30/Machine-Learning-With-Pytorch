# 🧠 Introduction to PyTorch

Before jumping into Google Colab coding, this document provides an
overview of **PyTorch**, its history, design philosophy, and how it
compares with TensorFlow.

------------------------------------------------------------------------

## 1. History of PyTorch

-   **First Release:** 2016\
-   **Developed by:** Facebook AI Research (FAIR), now Meta\
-   Designed to make deep learning:
    -   Easier to learn
    -   Flexible for research
    -   Fully integrated with Python

PyTorch quickly became the most popular deep learning framework in
academic research.

Official Website:\
https://pytorch.org

------------------------------------------------------------------------

## 2. What is Torch? (The Origin)

Before PyTorch, there was **Torch**.

-   Created around **2002**
-   Written in **Lua programming language**
-   Widely used in machine learning research

### Problem

-   Lua was unfamiliar to most developers
-   Difficult integration with Python ecosystem

### Solution

Rebuild Torch concepts using Python → **PyTorch**

------------------------------------------------------------------------

## 3. Facebook / Meta Connection

PyTorch was developed internally at Facebook to support:

-   Computer Vision
-   Recommendation Systems
-   Natural Language Processing

Meta later open-sourced PyTorch to accelerate AI innovation.

Today PyTorch development is supported by the **PyTorch Foundation**.

------------------------------------------------------------------------

## 4. GPU-Ready Tensor Library

At its core, PyTorch is a **tensor computation library**.

A tensor is a multidimensional array similar to:

-   Scalars (0D)
-   Vectors (1D)
-   Matrices (2D)
-   Higher dimensional data

PyTorch supports GPU acceleration using CUDA.

### CPU Example

    Computation happens sequentially

### GPU Example

    Thousands of operations run in parallel

CUDA Information:\
https://developer.nvidia.com/cuda-zone

------------------------------------------------------------------------

## 5. Tight Python Integration

PyTorch is deeply integrated with Python.

Design philosophy: - Similar usage to NumPy - Uses normal Python
syntax - Works naturally with Python libraries

NumPy: https://numpy.org

If you understand NumPy arrays, learning PyTorch tensors becomes much
easier.

------------------------------------------------------------------------

## 6. PyTorch as a Deep Learning Framework

### Automatic Differentiation (Autograd)

PyTorch automatically computes gradients needed for training neural
networks.

Process:

    Forward Pass → Operations Recorded
    Backward Pass → Gradients Computed Automatically

Documentation: https://pytorch.org/docs/stable/autograd.html

------------------------------------------------------------------------

### Dynamic Neural Networks

Neural networks can change during execution.

Example idea:

``` python
if condition:
    use_layer_A()
else:
    use_layer_B()
```

This flexibility is extremely useful for research experimentation.

------------------------------------------------------------------------

## 7. Imperative Execution

PyTorch uses **imperative execution**.

Meaning: - Code runs immediately - No compilation step required - Easy
debugging

Workflow:

    Write Code → Run → See Result

Unlike older frameworks, there is no separate build phase.

------------------------------------------------------------------------

## 8. Easy Extensibility

Developers can easily create:

-   Custom neural network layers
-   Loss functions
-   Optimizers
-   Experimental models

Example:

``` python
class MyLayer(nn.Module):
    pass
```

This makes PyTorch highly extensible.

------------------------------------------------------------------------

# ⚖️ TensorFlow vs PyTorch

------------------------------------------------------------------------

## What is TensorFlow?

TensorFlow is a machine learning framework developed by Google.

-   **First Release:** 2015
-   Designed originally for large-scale production systems

Official Website: https://www.tensorflow.org

------------------------------------------------------------------------

## Framework Timeline

  Framework    Release Year
  ------------ --------------
  Torch        2002
  TensorFlow   2015
  PyTorch      2016

------------------------------------------------------------------------

## Comparison Table

  Feature                 PyTorch           TensorFlow
  ----------------------- ----------------- -------------------------------
  Creator                 Meta (Facebook)   Google
  Release Year            2016              2015
  Execution Style         Imperative        Static Graph (early versions)
  Computation Graph       Dynamic           Static (originally)
  Debugging               Easy              More complex
  Python Integration      Excellent         Moderate
  CUDA GPU Support        Yes               Yes
  Visualization           Limited           TensorBoard
  Research Popularity     Very High         Medium
  Production Deployment   Growing           Strong

------------------------------------------------------------------------

## Mental Model

### TensorFlow (Early Design)

Plan computation graph first, then execute.

### PyTorch

Write Python code and execute immediately.

------------------------------------------------------------------------

# 🎯 Why We Use PyTorch

✅ Beginner friendly\
✅ Python-native\
✅ Research standard\
✅ Industry adoption\
✅ Excellent for experimentation

------------------------------------------------------------------------

# 🚀 Next Step: Google Colab

In upcoming labs, we will learn:

-   Tensor operations
-   GPU usage
-   Autograd
-   Neural networks
-   Training models

Google Colab: https://colab.research.google.com

------------------------------------------------------------------------

**Prepared for Machine Learning Lab**
