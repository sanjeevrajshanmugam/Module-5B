# NumPy Program: Column-wise Sorting of a 2D Array

## 🎯 Aim
To write a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

## 🧠 Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=0` to sort each column in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the column-wise sorted array.

## 🧾 Program:
```
import numpy as np
a=np.array(eval(input()))
print("Given array ")
b=np.sort(a, axis=0)
print(f" {a}")
print("")
print(b)
```
## Output:

<img width="751" height="645" alt="442577776-54cbbd43-337c-4faf-b4bd-38051413e1ae" src="https://github.com/user-attachments/assets/d87acf20-8635-4aa1-b592-25ee238604e6" />

## Result:
  Thus,the NumPy program that sorts the elements in each column of a given 2D array in ascending order is created successfully.
