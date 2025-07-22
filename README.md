# <h1>Python 12 Hourse </h1>

✅ 1. Multiplication Table Generator
num = int(input("Enter a number: "))
for i in range(1, 11):
    print(f"{num} x {i} = {num*i}")
✅ 2. Countdown Timer
import time
n = int(input("Countdown from: "))
while n > 0:
    print(n)
    time.sleep(1)
    n -= 1
print("Time's up!")
✅ 3. Sum of Digits
num = input("Enter a number: ")
sum = 0
for digit in num:
    sum += int(digit)
print("Sum of digits:", sum)
✅ 4. Prime Number Checker (1 to N)
n = int(input("Check primes up to: "))
for num in range(2, n+1):
    for i in range(2, num):
        if num % i == 0:
            break
    else:
        print(num, "is Prime")
✅ 5. Password Guesser
correct = "python123"
guess = ""
while guess != correct:
    guess = input("Enter password: ")
print("Access Granted")
✅ 6. Reverse a String
text = input("Enter a string: ")
reversed_text = ''
for char in text:
    reversed_text = char + reversed_text
print("Reversed:", reversed_text)
✅ 7. Find Factorial
n = int(input("Enter a number: "))
fact = 1
for i in range(1, n+1):
    fact *= i
print("Factorial:", fact)
✅ 8. Number Guessing Game
import random
num = random.randint(1, 10)
guess = 0
while guess != num:
    guess = int(input("Guess (1-10): "))
print("Correct!")
✅ 9. Pattern Printing (Right Triangle)
rows = 5
for i in range(1, rows+1):
    print("*" * i)
✅ 10. Palindrome Checker
text = input("Enter text: ")
reversed = text[::-1]
print("Palindrome!" if text == reversed else "Not a palindrome.")
✅ 11. FizzBuzz
for i in range(1, 101):
    if i%3==0 and i%5==0:
        print("FizzBuzz")
    elif i%3==0:
        print("Fizz")
    elif i%5==0:
        print("Buzz")
    else:
        print(i)
✅ 12. Average of N Numbers
n = int(input("How many numbers: "))
total = 0
for i in range(n):
    total += float(input(f"Enter number {i+1}: "))
print("Average:", total / n)
✅ 13. Armstrong Number Finder
for num in range(100, 1000):
    sum = 0
    temp = num
    while temp > 0:
        digit = temp % 10
        sum += digit ** 3
        temp //= 10
    if num == sum:
        print(num)
✅ 14. Multiples of a Number
n = int(input("Enter number: "))
for i in range(1, 11):
    print(n*i, end=" ")
✅ 15. Simple Interest Table
p = float(input("Principal: "))
r = float(input("Rate: "))
for t in range(1, 11):
    si = (p*r*t)/100
    print(f"Year {t}: Interest = {si}")
✅ 16. Vowel Counter
text = input("Enter text: ").lower()
count = 0
for char in text:
    if char in "aeiou":
        count += 1
print("Total vowels:", count)
✅ 17. Table of Squares
for i in range(1, 11):
    print(f"{i}^2 = {i*i}")
✅ 18. Remove Duplicates
items = [1, 2, 2, 3, 4, 4, 5]
unique = []
for i in items:
    if i not in unique:
        unique.append(i)
print(unique)
✅ 19. Fibonacci Series
n = int(input("How many terms: "))
a, b = 0, 1
for _ in range(n):
    print(a, end=" ")
    a, b = b, a + b
✅ 20. Number Pyramid
rows = 5
for i in range(1, rows+1):
    for j in range(1, i+1):
        print(j, end=" ")
    print()


