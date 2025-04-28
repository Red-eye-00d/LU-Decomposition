# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program and import the required libraries NumPy and SciPy.


 2. Read the input matrix (and input vector if solving equations).

 
3. Perform LU decomposition of the matrix using appropriate functions.


4. If solving equations, use the LU decomposition to find the solution vector.

5. Display the result (L and U matrices or the solution vector).



## Program:
(i) To find the L and U matrix
```python
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
/*
Program to find the L and U matrix.
Developed by: SUDHARSANAN U
RegisterNumber: 212224230276
*/
```
(ii) To find the LU Decomposition of a matrix
```python
import numpy as np
from scipy.linalg import lu_factor, lu_solve
A = np.array(eval(input()))
b = np.array(eval(input()))
lu, piv = lu_factor(A)
X = lu_solve((lu, piv),b)
print(X)
/*
Program to find the LU Decomposition of a matrix.
Developed by: SUDHARSANAN U
RegisterNumber: 212224230276
*/
```

## Output:
![lu decomposition]()

![image](https://github.com/user-attachments/assets/a677a6c8-c945-48f0-be1d-06494dcdb729)

![image](https://github.com/user-attachments/assets/64b98000-f700-43c2-969e-a2538d6b4399)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.
