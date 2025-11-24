# NumPy Program: Replace the Second Column in a 2D Array

## 🎯 Aim
To write a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

## 🧠 Algorithm
1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Get a 2D NumPy array and a new column (as another array) from the user.
3. **Delete Column**: Use `np.delete()` to remove the second column (index 1) from the original array.
4. **Insert Column**: Use `np.insert()` to insert the new column at the second column's original position.
5. **Display Result**: Print the updated array with the replaced column.

## 🧾 Program:
```
import numpy as np
a=np.array(eval(input()))
b=np.array(eval(input()))
print('Printing Original array')
print(a)
print('Array after deleting column 2 on axis 1')
c=np.delete(a,1,axis=1)
print(c)
print('Array after inserting column 2 on axis 1')
d=np.insert(c,1,b,axis=1)
print(d)
```
## Output:

<img width="1176" height="848" alt="442579661-db6261df-79e3-4772-9ec7-e3eb51383b4b" src="https://github.com/user-attachments/assets/e0cd83db-66e5-400c-9c37-3ec10ddfa30f" />

## Result:
  Thus,the NumPy program that deletes the second column from a given 2D array and inserts a new column at the same position is created successfully.
