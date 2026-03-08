# Tensor Operations Lab
Learn how to manipulate tensors using common PyTorch operations. By the end of this lab you should understand:

- element-wise operations
- matrix multiplication
- reshaping tensors
- broadcasting
- reduction operations

##  Element-wise Operations
Create two tensors:
```
A = [[1,2],
     [3,4]]

B = [[5,6],
     [7,8]]
```
### Exercise 1

Create tensors A and B. Then compute:
```
A + B
A - B
A * B
```
##  Matrix Multiplication
In machine learning we often multiply matrices.

### Exercise 2
Compute the matrix multiplication of:
```
A = [[1,2],
     [3,4]]

B = [[5,6],
     [7,8]]
```

Try two methods:
```
torch.matmul()
@
```
##  Tensor Shape, Size
Every tensor has a shape and Size.

### Exercise 3

Check the shape and size of tensor ```A```.

##  Reshaping Tensors
We can reshape tensors using view().

### Exercise 4

Create a tensor: ```[1,2,3,4,5,6]```.

Reshape it into a ```2 x 3``` tensor.

##  Reduction Operations
These operations summarize values.

### Exercise 5

Given: ```t = [1,2,3,4,5]```.

Find:

```
- sum
- mean
- max
- min
```  
##  Broadcasting
Broadcasting allows tensors of different shapes to operate together.

### Exercise 6
Example:
```
[1,2,3]
+
10
```
Create tensor:```[1,2,3]```and add 10.

##  Challenge Exercise

Create a tensor:

``` [[1,2,3], [4,5,6]]```.

Tasks:

1️⃣ Multiply the tensor by 2
2️⃣ Compute the row sum
3️⃣ Reshape it into ``` 3 x 2 ```
