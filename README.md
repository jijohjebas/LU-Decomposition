# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.Start the program
2.Import the necessary libraries(numpy,scipy.linalg)
3.Define the matrix using numpy
4.Use lu(),lu_solve(),lu_factor() to get the solutions
5.End the program
## Program:
(i) To find the L and U matrix
```
#Program to find L and U matrix using LU decomposition.
#Developed by: Jijo H Jebas
#RegisterNumber: 212225040156
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
#Program to solve a matrix using LU decomposition.
#Developed by: Jijo H Jebas
#RegisterNumber: 212225040156
# To print X matrix (solution to the equations)
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,pivot=lu_factor(A)
x=lu_solve((lu,pivot), B)
print(x)
```

## Output:
<img width="838" height="927" alt="image" src="https://github.com/user-attachments/assets/91adef02-245e-48d6-bf66-b1e357ab5a9b" />

<img width="771" height="699" alt="image" src="https://github.com/user-attachments/assets/417100e1-cb25-41bf-9825-d14ed990974d" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

