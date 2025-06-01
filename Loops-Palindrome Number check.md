## Loops in Python: Palindrome Number Checker

## 🎯 Aim
To write a Python program that checks whether a given number is a **palindrome** using loops.

## 🧠 Algorithm
1. Get input from the user and assign it to a variable `num`.
2. Assign the value of `num` to a temporary variable `temp`.
3. Initialize a variable `rev` to 0 (used to store the reversed number).
4. Use a `while` loop to reverse the digits:
   - While `temp > 0`:
     - `rev = (10 * rev) + temp % 10`
     - `temp = temp // 10`
5. After the loop, compare `rev` with `num`:
   - If equal, print that the number is a palindrome.
   - Else, print that it is not a palindrome.

## 🧾 Program
```
a=int(input())
num=a
rev=0
while(num>0):
    digit=num%10
    rev=rev*10+digit
    num//=10
if rev==a:
    print("The given number {} is a Palindrome".format(a))
else:
    print("The given number {} is not a palindrome".format(a))
```
## Output
![image](https://github.com/user-attachments/assets/b1028859-b56a-470a-924c-3f0d9d94203c)

## Result
Thus the program has been successfully executed.
