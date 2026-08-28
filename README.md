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
'''Program to solve a matrix using LU decomposition.
Developed by:Sherlin Jenifa VS
RegisterNumber:212225230263
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
Developed by: Sherlin Jenifa VS
RegisterNumber:212225230263
'''

# To print X matrix (solution to the equations)
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"

import numpy as np
from scipy.linalg import lu_factor,lu_solve

A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),b)
print(X)

```

## Output:
<img width="1072" height="763" alt="Screenshot 2026-08-28 131923" src="https://github.com/user-attachments/assets/ae0fe9fc-8467-459b-b003-d062dc47afcb" />
<img width="1090" height="791" alt="Screenshot 2026-08-28 131955" src="https://github.com/user-attachments/assets/473f814a-3c05-45a7-8b4c-e9af4b83271c" />
<img width="1196" height="721" alt="Screenshot 2026-08-28 131941" src="https://github.com/user-attachments/assets/3662a2b2-753d-4391-90c4-be3d03eec371" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

