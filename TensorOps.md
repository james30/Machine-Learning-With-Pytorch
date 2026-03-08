# Tensor Operations
Learn how to manipulate tensors using common PyTorch operations. By the end of this lab you should understand:

- Element-wise Operations
- Matrix Multiplication
- Reduction operations
- Broadcasting
- Shaping & Manipulation

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
##  Reduction Operations
These operations summarize values.

### Exercise 3

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

### Exercise 4
Example:
```
[1,2,3]
+
10
```
Create tensor:```[1,2,3]```and add 10.

##  Tensor Shape, Size
Every tensor has a shape and Size.

### Exercise 5

Check the shape and size of tensor ```A```.

##  Tensors Shaping & Manipulation

We can reshape tensors using view().

### Exercise 6

Create a tensor: ```x = [1,2,3,4,5,6]```.

- Reshape it into a ```2 x 3``` tensor.
- Transposes x
- Unsqueeze() and Squeeze()
- Cat() and Stack()
- Permute()

##  Challenge Exercise

Create a tensor:

``` [[1,2,3], [4,5,6]]```.

Tasks:

- Multiply the tensor by 2
- Compute the row sum
- Reshape it into ``` 3 x 2 ```
