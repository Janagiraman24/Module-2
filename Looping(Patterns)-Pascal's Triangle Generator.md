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
def pascal_triangle(n):
    for i in range(n):
        num = 1  # First element in every row is 1
        print(" " * (n - i-1), end="")  # Center alignment
        
        for j in range(i + 1):
            print(num, end=" ")  
            num = num * (i - j) // (j + 1)  # Compute next number in row
        
        print()  # Move to the next line
rows = int(input())
pascal_triangle(rows)
```
## Sample Output
![image](https://github.com/user-attachments/assets/877f7eda-7eb8-4631-af6a-2778ace37328)

## Result
Thus the program has been successfully executed.
