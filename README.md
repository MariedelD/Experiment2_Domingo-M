# Experiment 2: Numerical Python (NumPy)

**Submitted by:** Mariedel O. Domingo  

## I. Introduction

### Intended Learning Outcomes
- In this experiment, the primary objective is to develop a Python code within the Jupyter notebook, utilizing the Numpy library to address the provided problems.

## II. Instructions

### Problem 1: **Normalization Problem**

Normalization is a basic data preprocessing technique involving:
- **Centering**: Subtracting the mean from each data point.
- **Scaling**: Dividing by the standard deviation.

**Mathematically, normalization can be expressed as:**

#### Z = (matrix - mean)/standard_deviation. 

#### **Tasks:**
1. Generate a random 5×5 array.
2. Normalize it using the formula above.
3. Save the normalized array to a file named `X_normalized.npy`.

---

### Problem 2: **Divisible by 3 Problem**

#### **Tasks:**
1. Create a 10×10 NumPy array containing the squares of the first 100 positive integers.
2. Identify elements divisible by 3.
3. Save the resulting array to a file named `div_by_3.npy`.

---

## III. Solutions

---

### Problem 1: Normalization Problem

**Import the required library:**

```python
import numpy as np
```
#### Step 1: Create a random 5×5 array
```python
x = np.random.random((5, 5))
```

#### Step 2: Normalize the array
```python
 X_normalized = (x-x.mean() / x. std()
```

#### Step 3: Save the normalized array
```python
np. save ('X_normalized.npy', X_normalized) 
```

#### Step 4: Display the results
```python
print ("The Matrix: \n\n", x)
print ("\nThe Mean: ", x.mean ())
print("The Standard Deviation:", x.std())
print("\n The Normalized Values: \n", X_normalized)
```

#### OUTPUT:

<img width="591" height="371" alt="image" src="https://github.com/user-attachments/assets/7fefb59b-fcc1-45ab-8853-821717ed04dc" />


### Problem 2: DIVISIBLE BY 3 PROBLEM

#### Import the required library:
```python
import numpy as np
```

#### Step 1: Create an array of squares from 1 to 100
```python
A = np-arange (1, 101) **2
```

#### Step 2: Reshape into a 10×10 array
```python
A = A. reshape (10, 10)
```
#### Step 3: Filter elements divisible by 3
```python
div_by_3 = A[A % 3 == 0]
```

#### Step 4: Save the filtered results
```python
np.save('div_by_3.npy', div_by_3)
```

#### Display the original array and the filtered result 

```python
print ("The Original Array: In\n", A)
print ("\nThe values that are divisible by 3: In\n", div_by_3)
```

#### OUTPUT:
<img width="683" height="351" alt="image" src="https://github.com/user-attachments/assets/f6bb2ca9-4eae-4e1d-8a3e-67dd76a04bfc" />
