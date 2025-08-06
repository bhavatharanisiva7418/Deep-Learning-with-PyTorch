## PyTorch Basics Exercises
## AIM:
Write a Python program using PyTorch that performs the following tasks:

## Software Required:
Python 3.x
PyTorch
Jupyter Notebook (for interactive development and execution)
## Algorithm:

## Name: BHAVATHARANI S
## Register Number: 212223230032
## Step 1:

Perform standard imports

Import torch and NumPy.
```
# CODE HERE
import torch
import numpy as np
```

## Step 2:
Set the random seed for NumPy and PyTorch both to 42.
```
# YOUR CODE HERE
seed = 42
np.random.seed(seed)
torch.manual_seed(seed)
```

## Step 3:
Create a NumPy array called arr that contains 6 random integers between 0 (inclusive) and 5 (exclusive).
```
# YOUR CODE HERE
arr = np.random.randint(0, 5, size=6)
print(arr)
```

## Step 4:
Create a tensor x from the array above.
```
# YOUR CODE HERE
x = torch.tensor(arr, dtype=torch.int32)
print(x)
```

## Step 5:
Change the dtype of x from int32 to int64.
```
# YOUR CODE HERE
x = x.type(torch.int64)
print(x)
```

## Step 6:
Reshape x into a 3x2 tensor.
```
# YOUR CODE HERE
x = x.view(3, 2)
print(x)
```

## Step 7:
Return the right-hand column of tensor x.
```
# YOUR CODE HERE
right_column = x[:, 1].unsqueeze(1) 
print(right_column)
```

## Step 8:
Without changing x, return a tensor of square values of x.
```
# YOUR CODE HERE
x_squared = x ** 2
print(x_squared)
```

## Step 9:
Create a tensor y with the same number of elements as x, that can be matrix-multiplied with x.

Use PyTorch directly (not NumPy) to create a tensor of random integers between 0 (inclusive) and 5 (exclusive).
```
# YOUR CODE HERE

y = torch.randint(0, 5, (2, 3), dtype=torch.int64)
print(y)
```

## Step 10:
Find the matrix product of x and y.
```
# YOUR CODE HERE

result = torch.matmul(x, y)
print(result)
```

### Output:
i) Import and set up PyTorch and NumPy.

ii) Create and manipulate tensors.

iii) Perform matrix operations.

## Result:
Thus, the PyTorch tensor operations, including reshaping, dtype conversion, and matrix multiplication, were successfully performed using the Python program.
