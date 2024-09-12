## <center> EXPERIMENT 2: NUMERICAL PYTHON (NUMPY)

Name: Trangia, Klein Isshi G.

Section: 2ECE-D

Date Submitted: September 5, 2024

## 1. __NORMALIZATION PROBLEM__ : 
Normalization is one of the most basic preprocessing techniques in data analytics. This involves centering and scaling process. Centering means subtracting the data from the mean and scaling means dividing with its standard deviation. Mathematically, normalization can be expressed as:  𝑍 = 𝑋 − 𝑥̅  / 𝜎

In Python, element-wise mean and element-wise standard deviation can be obtained by using .mean() and .std() calls.

In this problem, create a random 5 x 5 ndarray and store it to variable X. Normalize X. Save your normalized ndarray as X_normalized.npy

import numpy as np

x = np.random.random((5,5))

print (x)

a = x.mean()

b = x.std()

normal = (x-a)/b

print (normal)

np.save ('X_normalized.npy',normal)

## EXPLANATION
- First, I used the import numpy as np to access the NumPy Library. I then proceed to use "x = np.random.random((5,5))" to produce a 5x5 array containing random sets of numbers. After printing it, I stored the mean formula in "a" and the standard deviation formula in "b". In the following code, I typed the normal formula, which is normal = (x-a)/b, and printed it again so that the normal value with respect to "x" will be shown.

## 2. __DIVISIBLE BY 3 PROBLEM__ :
Create the following 10 x 10 ndarray.

which are the squares of the first 100 positive integers.

From this ndarray, determine all the elements that are divisible by 3. Save the result as div_by_3.npy

k = np.arange(1,101)

i = np.square (k)

g = i.reshape (10,10)

print (g)

t = g [g%3==0]

print (t)

np.save ('div_by_3.npy',t)

## EXPLANATION
- For the second problem, I input "k = np.arange(1,101)" to produce an array with values of 1-100. I stored the code in "i" to square the values of 1-100 and then reshaped it into a 10x10 array which I stored in "g". After that, I printed the values and stored the code responsible for making the values divisible by 3 in "t" and printed it again.
