# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the numpy module to use the built in function for calculation.
2. Import the sys function. Get input from the user for the matrix i and j using for loop.
3. Check wheather the matrix of element is divisible by zero. If divisible by zero then print zero is detected. And further find the ratio of the matrix.
4. End the program.

## Program:
```
/*
Program to find the solution of a matrix using Gaussian Elimination.
Developed by: 
RegisterNumber: 

import numpy as np

import sys

n=int(input())

a=np.zeros((n,n+1))

x=np.zeros(n)

for i in range(n):

for j in range(n+1):

    a[i][j]=float(input())

for i in range(n):   
    
    if a[i][j]==0.0:
       
       sys.exit('divide by zero detected!')
    
    for j in range(i+1,n):
        
        ratio=a[j][i]/a[i][i]
        
        for k in range(n+1):
            
            a[j][k]=a[j][k]-ratio*a[i][k]

x[n-1]=a[n-1][n]/a[n-1][n-1]

for i in range(n-2,-1,-1):
    
    x[i]=a[i][n]
    
    for j in range(i+1,n):
        
        x[i]=x[i]-a[i][j]*x[j]
    
    x[i]=x[i]/a[i][i]

for i in range(n):
    
    print('X%d = %0.2f'%(i,x[i]),end=' ')
   
*/
```   
    
## Output:
![mex6](https://user-images.githubusercontent.com/117974950/213450106-4380625f-d4a7-4672-9b7c-c1ef387ce237.png)



## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

