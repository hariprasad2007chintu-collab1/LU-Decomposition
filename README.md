# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.Start the program and import the required library (numpy).
2.Initialize the matrix for which the LU decomposition needs to be found. 
3.Apply LU Decomposition. 
4.Display the results.
 
 
 

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: Hariprasad A
RegisterNumber: 212225240048
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
InputMatrix=np.array(eval(input()),dtype='i')
piv,Lmatrix,Umatrix=lu(InputMatrix)
print(Lmatrix)
print(Umatrix)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: Hariprasad A
RegisterNumber: 212225240048
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
Amatrix=np.array(eval(input()),dtype='i')
Bmatrix=np.array(eval(input()),dtype='i')
Xmatrix=lu_factor(Amatrix)
Solution=lu_solve(Xmatrix,Bmatrix)
print(Solution)
```

## Output:
![lu decomposition]()
<img width="1278" height="512" alt="Screenshot 2026-06-11 010507" src="https://github.com/user-attachments/assets/93699707-813f-41d2-9184-512a143dec2c" />

<img width="1366" height="347" alt="image" src="https://github.com/user-attachments/assets/8f223301-8822-4759-be7c-e58d2a3af66e" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

