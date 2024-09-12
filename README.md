#### <center> EXPERIMENT 2

## <center> NUMERICAL PYTHON (NUMPY)

### __NORMALIZATION PROBLEM__
import numpy as np

x = np.random.random((5,5))

print (x)

a = x.mean()

b = x.std()

normal = (x-a)/b

print (normal)

np.save ('X_normalized.npy',normal)

### __DIVISIBLE BY 3 PROBLEM__
k = np.arange(1,101)

i = np.square (k)

g = i.reshape (10,10)

print (g)

t = g [g%3==0]

print (t)

np.save ('div_by_3.npy',t)
