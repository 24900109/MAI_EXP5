# LU Decomposition 
## Name: KIRUTHIKA N
## Register Number: 212224230127

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
## Step 1:
Import required libraries (NumPy and SciPy) and read the input matrix A.

## Step 2:
Perform LU decomposition of matrix A and obtain L and U matrices.

## Step 3:
Display the L and U matrices to verify the decomposition.

## Step 4:
If required, read matrix/vector B and solve the system AX = B using LU factorization.

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: KIRUTHIKA N 
RegisterNumber: 212224230127
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"

import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: 
RegisterNumber: 
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1" 

import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,pivot=lu_factor(A)
x=lu_solve((lu,pivot),B)
print(x)
```

## Output:

<img width="1255" height="596" alt="5 1" src="https://github.com/user-attachments/assets/1fb2f82e-6bd6-4550-ba82-16866b654ed9" />

<img width="1248" height="332" alt="5 2" src="https://github.com/user-attachments/assets/5961f339-5357-4ee5-8c99-de6b6ef1dfc1" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.
