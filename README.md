# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
(i) To find the L and U matrix
* Import **NumPy** and required function from **SciPy**
* Define the input matrix ( A ) using NumPy array
* Apply LU decomposition using `lu(A)` to obtain ( P, L, U )
* Display ( L ) and ( U ) matrices

(ii) To find the LU Decomposition of a matrix
* Import **NumPy** and `lu_factor`, `lu_solve` from **SciPy**
* Define matrix ( A ) and right-hand side vector ( b )
* Apply `lu_factor(A)` to obtain LU matrix and pivot indices
* Use `lu_solve((lu, piv), b)` to compute the solution vector

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: V. HARINI
RegisterNumber: 212225040113
*/

import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U = lu(A)
print(L)
print(U)

```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: V. HARINI
RegisterNumber: 212225040113
*/

import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A = np.array(eval(input()))
b = np.array(eval(input()))
lu,piv = lu_factor(A)
X = lu_solve((lu,piv),b)
print(X)

```

## Output:
![lu decomposition]()

(i) To find the L and U matrix
<img width="1174" height="455" alt="Screenshot 2026-03-22 110331" src="https://github.com/user-attachments/assets/0742e729-ea61-4fee-834b-871ba58a516e" />

(ii) To find the LU Decomposition of a matrix
<img width="882" height="195" alt="Screenshot 2026-03-22 110444" src="https://github.com/user-attachments/assets/cc5f030b-3404-4fe1-be4b-7fc558552656" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

