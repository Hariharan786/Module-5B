# NumPy Program: Column-wise Sorting of a 2D Array

## 🎯 Aim
To write a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

## 🧠 Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=0` to sort each column in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the column-wise sorted array.

## 🧾 Program
```
import numpy as np

rows = int(input("Enter number of rows: "))
cols = int(input("Enter number of columns: "))

elements = []
for i in range(rows):
    row = list(map(int, input(f"Enter row {i+1} elements separated by space: ").split()))
    elements.append(row)

arr = np.array(elements)
sorted_arr = np.sort(arr, axis=0)

print("Original array:\n", arr)
print("Column-wise sorted array:\n", sorted_arr)
```

## Output
![alt text](<Screenshot 2025-10-20 170923.png>)
## Result
