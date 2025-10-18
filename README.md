# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
(i) To find the L and U matrix
1. Import NumPy as np and lu function from the SciPy.linalg module to perform matrix decomposition.
2. Get the matrix A as input from the user and convert it into a NumPy array.
3. Use the lu() function to decompose the matrix A into P, L, and U matrices
4. Display the L and U matrices as the output and end the program.

(ii) To find the LU Decomposition of a matrix
1. Import NumPy as np and the functions lu_factor and lu_solve from the SciPy.linalg module to solve linear equations using LU decomposition.
2. Take the coefficient matrix A and the constant matrix (or vector) b as input from the user and convert them into NumPy arrays.
3. Use the lu_factor() function to decompose the matrix A into LU form and store the result along with the pivot array piv.
4. Use the lu_solve() function with (lu, piv) and b to find the solution vector X, then display the result.


## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: A.RAFSHAAN AHMED
RegisterNumber: 212224230214
*/
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: sanjai ganth
RegisterNumber: 212224230244
*/
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),b)
print(X)
```

## Output:
(i) To find the L and U matrix
<img width="1221" height="562" alt="image" src="https://github.com/user-attachments/assets/f929e59d-a1ac-4b36-ba42-2480a59008a0" />



(ii) To find the LU Decomposition of a matrix
<img width="1026" height="170" alt="image" src="https://github.com/user-attachments/assets/0059e596-500e-491d-95a8-da5c088a3093" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

