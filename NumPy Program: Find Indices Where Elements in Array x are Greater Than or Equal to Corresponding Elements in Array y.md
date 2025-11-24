# # NumPy Program: Find Indices Where Elements in Array x are Greater Than or Equal to Corresponding Elements in Array y

## 🎯 Aim
To write a Python program using **NumPy** that finds the indices where elements in array `x` are greater than or equal to their corresponding elements in array `y`.

## 🧠 Algorithm
1. **Import NumPy**: Import the NumPy library.
2. **Define Arrays**: Define two NumPy arrays, `x` and `y`, with the same shape (i.e., same number of elements).
3. **Use Boolean Indexing**: 
   - `x > y` gives a boolean array where elements of `x` are greater than `y`.
   - `x == y` gives a boolean array where elements of `x` are equal to `y`.
4. **Find Indices**: Use `np.where()` to get the indices where the conditions `x >= y` are satisfied.
5. **Print Indices**: Print the indices where the condition holds true.

## 🧾 Program:
```
import numpy as np
X=np.array(eval(input()))
Y=np.array(eval(input()))
greater=np.where(X>Y)
print(greater)
equal=np.where(X==Y)
print(equal)
```
## Output:

<img width="842" height="371" alt="442578541-8584f72e-6aa3-4d03-94de-7be4657f6b5c" src="https://github.com/user-attachments/assets/a018ff0e-0a7c-4614-96e9-69fc7d82e28d" />

## Result:
   Thus,the Python program using NumPy that finds the indices where elements in array x are greater than or equal to their corresponding elements in array y is created successfully.
