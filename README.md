# Implementation of Univariate Linear Regression

Name : Alan Samuel Vedanayagam
Reg.No: 212223040012

## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Get the independent variable X and dependent variable Y.
2. Calculate the mean of the X -values and the mean of the Y -values.
3. Find the slope m of the line of best fit using the formula. 
<img width="231" alt="image" src="https://user-images.githubusercontent.com/93026020/192078527-b3b5ee3e-992f-46c4-865b-3b7ce4ac54ad.png">
4. Compute the y -intercept of the line by using the formula:
<img width="148" alt="image" src="https://user-images.githubusercontent.com/93026020/192078545-79d70b90-7e9d-4b85-9f8b-9d7548a4c5a4.png">
5. Use the slope m and the y -intercept to form the equation of the line.
6. Obtain the straight line equation Y=mX+b and plot the scatterplot.

## Program:
```
/*
Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: Alan Samuel Vedanayagam
RegisterNumber:  212223040012

import numpy as np
import matplotlib.pyplot as plt
X=np.array(eval(input()))
Y=np.array(eval(input()))
a=np.mean(X)
b=np.mean(Y)
num=0
denom=0
for i in range(len(X)):
    num+=(X[i]-a)*(Y[i]-b)
    denom+=(X[i]-a)**2
m=num/denom
c=b-m*a
print("The slope is ",m)
print("The y intercept is ",c)
yp=m*X+c
print("Line Equation",yp)
plt.scatter(X,Y)
plt.plot(X,yp,color='red')
plt.show()
*/
```

## Output:

![image](https://github.com/user-attachments/assets/fb5d630e-4cad-4fe7-874b-1ee4bd99ae77)
![image](https://github.com/user-attachments/assets/ac4f4617-64ef-46e5-a333-682896bf2ac6)
![image](https://github.com/user-attachments/assets/000d235c-4761-4b32-8ce6-ce2e4506cbfa)


## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
