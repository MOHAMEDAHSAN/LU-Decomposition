# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
#### (i) To find the L and U matrix :
1. Import lu from scipy.linalg
2. Get the matrix from the user as input
3. Using lu() we get Pivot, L Matrix & U Matrix 
4. Display the L Matrix & U Matrix using print()

## Program:
#### (i) To find the L and U matrix :
~~~Python
'''Program to find L and U matrix using LU decomposition.
Developed by: MOHAMEDAHSAN
RegisterNumber: 23001044
'''
from scipy.linalg import lu
A=eval(input())
P,L,U=lu(A)
print(L,U,sep='\n')
~~~
#### (ii) To find the LU Decomposition of a matrix
~~~Python
'''Program to solve a matrix using LU decomposition.
Developed by: MOHAMEDAHSAN
RegisterNumber: 23001044
'''

# To print X matrix (solution to the equations)
from scipy.linalg import lu_factor,lu_solve
A=eval(input())
B=eval(input())
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),B)
print(X)
~~~
## Output:
#### (i) To find the L and U matrix :
![lu](/lu.png)
#### (ii) To find the LU Decomposition of a matrix
![lusolve](/solvelu.png)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

