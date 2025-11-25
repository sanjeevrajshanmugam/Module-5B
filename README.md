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


# Pandas Program: Create and Display a DataFrame with Custom Index Labels

## 🎯 Aim

To create and display a **DataFrame** using the **Pandas** library in Python from a given dictionary, and apply specific index labels to the rows.

---

## 🧠 Algorithm

1. **Import Libraries**: Import the required libraries – `pandas` and `numpy`.
2. **Create Dictionary**: Define a dictionary `exam_data` with keys: `'name'`, `'score'`, `'attempts'`, and `'qualify'`.
3. **Index Labels**: Create a list of custom index labels called `labels`.
4. **Create DataFrame**: Use `pd.DataFrame()` to create the DataFrame by passing the dictionary and index labels.
5. **Display Output**: Display the DataFrame using `print()` or by simply calling the DataFrame variable.

---

## 💻 Program:
```
import pandas as pd
import numpy as np
data = {
    'name': ['Anastasia', 'Dima', 'Katherine', 'James', 'Emily', 
             'Michael', 'Matthew', 'Laura', 'Kevin', 'Jonas'],
    'score': [12.5, 9, 16.5, np.nan, 9, 20, 14.5, np.nan, 8, 19],
    'attempts': [1, 3, 2, 3, 2, 3, 1, 1, 2, 1],
    'qualify': ['yes', 'no', 'yes', 'no', 'no', 
                'yes', 'yes', 'no', 'no', 'yes']
}
labels = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j']
df = pd.DataFrame(data, index=labels)
print(df)
```
## Output:

<img width="1201" height="528" alt="442581481-3bb5d6af-d37a-4bea-9564-a233a2d9b44e" src="https://github.com/user-attachments/assets/6f469787-c0f4-4558-8dd8-11f713c3c025" />

## Result:
  Thus,the Python program create and display a DataFrame using the Pandas library in Python from a given dictionary, and apply specific index labels to the rows is created successfully.


# 🧪 Pandas Program: Join Two DataFrames Along Rows

## 🎯 AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

---

## 🧠 ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.

---

## 💻 Program:
```
import pandas as pd
a=pd.DataFrame(eval(input()))
b=pd.DataFrame(eval(input()))
print("Original DataFrames:")
print(a)
print("-------------------------------------")
print(b)
print()
print("Join the said two dataframes along columns:")
c=pd.concat([a,b],axis=1)
print(c)
```
## Output:

<img width="1329" height="555" alt="443927659-155125c1-bd10-4d8d-807d-c97b345ce72e" src="https://github.com/user-attachments/assets/17025809-d401-4cfb-99d2-08dcb0282955" />

## Result:
  Thus,the Python program using Pandas to join two DataFrames along rows (row-wise concatenation) and assign all data to a new DataFrame is created successfully.




## REVIEW PAGE FOR MODULE


<img width="1919" height="877" alt="image" src="https://github.com/user-attachments/assets/ab56f53f-e28a-4cfc-9e80-c5cc9c6150a5" />

  
