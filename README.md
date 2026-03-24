# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program and import necessary libraries (numpy, scipy.linalg).
2. Input/define matrix A and vector b, and convert them into NumPy arrays.
3. Perform LU decomposition of matrix A using lu() to obtain matrices P, L, and U.
4. Apply LU factorization and solve the system using lu_factor() and lu_solve() to compute solution vector x.
5. Display matrices L, U and solution vector x, then stop the program.

## Program:
(i) To find the L and U matrix
```

Program to find the L and U matrix.
Developed by: Kabilan s
RegisterNumber: 212225230119

import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P, L, U =lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```

Program to find the LU Decomposition of a matrix.
Developed by: Kabilan S
RegisterNumber: 212225230119


import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array([[3, 2, 7], [2, 3, 1], [3, 4, 1]])
b=np.array([4, 5, 7])
lu, piv = lu_factor(A)
x=lu_solve((lu,piv),b)
print(x)

```

## Output:
<img width="1874" height="929" alt="Screenshot 2026-03-24 201041" src="https://github.com/user-attachments/assets/30d060db-6b60-4419-b908-82860288dc71" />
<img width="1870" height="905" alt="Screenshot 2026-03-24 201053" src="https://github.com/user-attachments/assets/f74b0392-e73e-4ed5-b623-3434ba503984" />
<img width="1863" height="908" alt="Screenshot 2026-03-24 201104" src="https://github.com/user-attachments/assets/7ac8cf38-c4a9-4347-abef-8a90febb7f76" />




## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

