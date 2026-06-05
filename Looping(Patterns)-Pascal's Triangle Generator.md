# 🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.

---

## 🎯 Aim

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.

---

## 🧠 Algorithm

1. Start the program.
2. Input the number of rows from the user.
3. Loop from 0 to the number of rows.
4. For each row:
   - Print appropriate spaces to shape the triangle.
   - Compute values using the formula:  
     \[
     C(n, k) = \frac{n!}{k!(n-k)!}
     \]
5. Print all rows of Pascal’s Triangle.
6. End the program.

---

## 🧪 Program

```
from math import factorial

rows = int(input("Enter the number of rows: "))

for i in range(rows):
    for j in range(rows - i - 1):
        print(" ", end="")

    for j in range(i + 1):
        value = factorial(i) // (factorial(j) * factorial(i - j))
        print(value, end=" ")

    print()
```

## Sample Output

<img width="363" height="157" alt="601365714-74b096a2-ee7d-4d3d-851d-ceef130dfc03" src="https://github.com/user-attachments/assets/4233afdc-901b-41fd-9972-e4241e27f7fd" />

## Result
Thus, the Python program to generate Pascal’s Triangle using numbers for the given number of rows was executed successfully and the output was verified.
