## PyTorch Basics Exercises

## Name: BHAVATHARANI S
## Register Number: 212223230032

## AIM:
Write a Python program using PyTorch that performs the following tasks:

## Software Required:
Python 3.x
PyTorch
Jupyter Notebook (for interactive development and execution)
## Algorithm:
## Step 1:

Perform standard imports

Import torch and NumPy.
```
import torch
import numpy as np
```

## Step 2:
Set the random seed for NumPy and PyTorch both to 42.
```
seed = 42
np.random.seed(seed)
torch.manual_seed(seed)
```

## Step 3:
Create a NumPy array called arr that contains 6 random integers between 0 (inclusive) and 5 (exclusive).
```
arr = np.random.randint(0, 5, size=6)
print(arr)
```

## Step 4:
Create a tensor x from the array above.
```
x = torch.tensor(arr, dtype=torch.int32)
print(x)
```

## Step 5:
Change the dtype of x from int32 to int64.
```
x = x.type(torch.int64)
print(x)
```

## Step 6:
Reshape x into a 3x2 tensor.
```
x = x.view(3, 2)
print(x)
```

## Step 7:
Return the right-hand column of tensor x.
```
right_column = x[:, 1].unsqueeze(1) 
print(right_column)
```

## Step 8:
Without changing x, return a tensor of square values of x.
```
x_squared = x ** 2
print(x_squared)
```

## Step 9:
Create a tensor y with the same number of elements as x, that can be matrix-multiplied with x.

Use PyTorch directly (not NumPy) to create a tensor of random integers between 0 (inclusive) and 5 (exclusive).
```


y = torch.randint(0, 5, (2, 3), dtype=torch.int64)
print(y)
```

## Step 10:
Find the matrix product of x and y.
```


result = torch.matmul(x, y)
print(result)
```

### Output:
i) Import and set up PyTorch and NumPy.

<img width="477" height="95" alt="image" src="https://github.com/user-attachments/assets/93bd8a05-99f1-4789-a6be-5188cf90cf54" />



ii) Create and manipulate tensors.

iii) Perform matrix operations.

## Result:
Thus, the PyTorch tensor operations, including reshaping, dtype conversion, and matrix multiplication, were successfully performed using the Python program.
