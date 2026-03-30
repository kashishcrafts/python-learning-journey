# Chapter 7 Practice Set

# Q1. Write a program to print multiplication table of a given number using for loop.
n = 5
for i in range(1, 11):
    print(f"{n} x {i} = {n*i}")

print()

# Q2. Write a program to greet all the person names stored in a list 'l'
# and which starts with S.
l = ["Harry", "Soham", "Sachin", "Rahul"]

for name in l:
    if name.startswith("S"):
        print("Hello", name)

print()

# Q3. Attempt problem 1 using while loop.
n = 5
i = 1
while i <= 10:
    print(f"{n} x {i} = {n*i}")
    i += 1

print()

# Q4. Write a program to find whether a given number is prime or not.
n = 29
is_prime = True

if n < 2:
    is_prime = False
else:
    for i in range(2, n):
        if n % i == 0:
            is_prime = False
            break

print("Prime" if is_prime else "Not Prime")

print()

# Q5. Write a program to find the sum of first n natural numbers using while loop.
n = 5
i = 1
total = 0

while i <= n:
    total += i
    i += 1

print("Sum =", total)

print()

# Q6. Write a program to calculate the factorial of a given number using for loop.
n = 5
factorial = 1

for i in range(1, n + 1):
    factorial *= i

print("Factorial =", factorial)

print()

# Q7. Write a program to print the following star pattern for n = 3:
#   *
#  ***
# *****

n = 3
for i in range(1, n + 1):
    print(" " * (n - i), end="")
    print("*" * (2 * i - 1))

print()

# Q8. Write a program to print the following star pattern for n = 3:
# *
# **
# ***

n = 3
for i in range(1, n + 1):
    print("*" * i)

print()

# Q9. Write a program to print the following star pattern for n = 3:
# * * *
# *   *
# * * *

n = 3
for i in range(1, n + 1):
    if i == 1 or i == n:
        print("* " * n)
    else:
        print("*" + " " * (2 * n - 3) + "*")

print()

# Q10. Write a program to print multiplication table of n using for loops in reversed order.
n = 5
for i in range(10, 0, -1):
    print(f"{n} x {i} = {n*i}")


