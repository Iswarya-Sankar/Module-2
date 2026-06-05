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
num = int(input("Enter a number: "))

temp = num
rev = 0

while temp > 0:
    rev = (10 * rev) + (temp % 10)
    temp = temp // 10

if rev == num:
    print("Palindrome")
else:
    print("Not Palindrome")
```
## Output

<img width="232" height="70" alt="601365964-34ade2bb-85cf-4783-8b2f-ec5940b24470" src="https://github.com/user-attachments/assets/7519eca9-7430-42ae-b45d-50c2ba503d3e" />

## Result

Thus, the Python program to check whether a given number is a palindrome using loops was executed successfully and the output was verified.
