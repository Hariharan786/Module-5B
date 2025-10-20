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

## 💻 Program

```
import pandas as pd

student_data1 = {
    'name': ['Alex', 'Amy', 'Allen'],
    'score': [85, 90, 88],
    'age': [20, 21, 19]
}

student_data2 = {
    'name': ['Bob', 'Bella', 'Brian'],
    'score': [82, 95, 89],
    'age': [22, 20, 23]
}

df1 = pd.DataFrame(student_data1)
df2 = pd.DataFrame(student_data2)

combined_df = pd.concat([df1, df2], axis=0)

print(combined_df)
```

## Output
![alt text](<Screenshot 2025-10-20 172108.png>)
## Result
