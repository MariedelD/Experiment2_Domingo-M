# Experiment2_Domingo-M

Experiment 2: Numericak Python (NumPy)
Submitted By: DOMINGO, Mariedel O.

I. INTRODUCTION

Intended Learning Outcomes
- In this experiment, the primary objective is to develop a Python code within the Jupyter notebook, utilizing the Numpy library to address the provided problems.


II. INSTRUCTIONS

Problem 1: NORMALIZATION PROBLEM

Normalization is one of the most basic preprocessing techniques in data analytics. This involves centering and scaling process. Centering means subtracting the data from the mean and scaling means dividing with its standard deviation. 

Mathematically, normalization can be expressed as: 

Z = (matrix - mean)/standard_deviation. 

Task
1. Make a random 5×5 array.
2. Normalize it using the formula above.
3. Save the normalized array to a file named X_normalized.npy.

Problem 2: DIVISIBLE BY 3 PROBLEM

Task
1. Create a 10 x 10 NumPy array of the squares of the first 100 positive integers.
2. From this array, find all elements divisible by 3.
3. Save the result (those divisible by 3) as a .npy file called div_by_3.npy.

II. SOLUTIONS

Problem 1: NORMALIZATION PROBLEM

 **$\color{lightblue}{Utilize\ the\ following\ import\ convention}$** to access the library that will be used throughout the program.

```python
import numpy as np
```

Next by utilizing the np.random.random function make a random 5×5 array the data in the created array will be utilized this will be the one calculatexd


```python
 x = np.random.random([5,5])
```

To calculatevthe normalized value, create a function stored in X_normalized that will help calculate the arrat

```python
 X_normalized = (x-x.mean() / x. std()
```

Save the normalized values by utilizing the np.save function

```python
np. save ('X_normalized.npy', X_normalized) 
```


The following functions will display the matrix

```python
print ("The Matrix: \n\n", x)
print ("\nThe Mean: ", x.mean ())
print("The Standard Deviation:", x.std())
print("\n The Normalized Values: \n", X_normalized)
```

OUTPUT:

<img width="591" height="371" alt="image" src="https://github.com/user-attachments/assets/7fefb59b-fcc1-45ab-8853-821717ed04dc" />


Problem 2: DIVISIBLE BY 3 PROBLEM

PROBLEM

 **$\color{lightblue}{Utilize\ the\ following\ import\ convention}$** to access the library that will be used throughout the program.

```python
import numpy as np
```

This function creates ndarrays withing a specific range

```python
A = np-arange (1, 101) **2
```

Reshape into 10x10 arrays

```python
A = A. reshape (10, 10)
```

This function will filter the elements that are divisible by 3

```python
div_by_3 = A[A % 3 == 0]
```

Save the the result as div_by_3.npy 

```python
np.save('div_by_3.npy', div_by_3)
```

Display the original array and the filtered result 

```python
print ("The Original Array: In\n", A)
print ("\nThe values that are divisible by 3: In\n", div_by_3)
```

OUTPUT:
<img width="683" height="351" alt="image" src="https://github.com/user-attachments/assets/f6bb2ca9-4eae-4e1d-8a3e-67dd76a04bfc" />
