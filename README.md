# Correlation and Regression for Data Analysis
# Aim : 

To analyse given data using  coeffificient of correlation and regression line.
![image](https://user-images.githubusercontent.com/104613195/168224136-d6b64e64-7d3d-4775-9337-c8f96fe41f2d.png)


# Software required :  

Python

# Theory:

Correlation describes the strength of an association between two variables, and is completely symmetrical, the correlation between A and B is the same as the correlation between B and A. However, if the two variables are related it means that when one changes by a certain amount the other changes on an average by a certain amount.  

If y represents the dependent variable and x the independent variable, this relationship is described as the regression of y on x. The relationship can be represented by a simple equation called the regression equation. The regression equation representing how much y changes with any given change of x can be used to construct a regression line on a scatter diagram, and in the simplest case this is assumed to be a straight line.

# Procedure :

![image](https://user-images.githubusercontent.com/104613195/168225866-ac8f6610-bdc3-4ac2-a24e-2b24ba08e189.png)

# Program
```
import numpy as np 
import math
x=[25,28,35,32,31,36,29,38,34,32]
y=[43,46,49,41,36,32,31,30,33,39]
Sx=0
Sy=0
Sxy=0
Sx2=0
Sy2=0
for i in range(0,10):
    Sx=Sx+x[i]
    Sy=Sy+y[i]
    Sxy=Sxy+x[i]*y[i]
    Sx2=Sx2+x[i]**2
    Sy2=Sy2+y[i]**2
    N=10
r=(N*Sxy-Sx*Sy)/(math.sqrt(N*Sx2-Sx*2)*math.sqrt(N*Sy2-Sy*2))
print("The Correlation coefficient is %0.3f"%r)


```
# output :
![Screenshot 2022-05-18 114510](https://user-images.githubusercontent.com/75234790/168970562-a90d7de7-94f8-4e5d-afb6-49ecc504cd40.png)




# Results : 
Hence a program has been implemented to find marginal distributions and correation coefficient of joint probability mass funcition of two dimensional random variables
