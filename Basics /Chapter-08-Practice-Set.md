# Chapter 8 Practice Set - Functions

# Q1: Create a function to find greatest of 3 numbers

def greatest(a, b, c):
    return max(a, b, c)

print(greatest(10, 20, 15))

# Input: 10, 20, 15
# Output: 20


# Q2: Convert Celsius to Fahrenheit

def c_to_f(c):
    return (c * 9/5) + 32

print(c_to_f(0))

# Input: 0
# Output: 32.0


# Q3: Prevent print() from printing new line

print("Hello", end="")
print("World")

# Output: HelloWorld


# Q4: Recursive function to find sum of first n natural numbers

def sum_n(n):
    if n == 0:
        return 0
    return n + sum_n(n-1)

print(sum_n(5))

# Input: 5
# Output: 15


# Q5: Print star pattern

def pattern(n):
    for i in range(n):
        print("*" * (n-i))

pattern(3)

# Input: 3
# Output:
# ***
# **
# *


# Q6: Convert inches to cm

def inch_to_cm(inch):
    return inch * 2.54

print(inch_to_cm(10))

# Input: 10
# Output: 25.4


# Q7: Remove word and strip spaces

def remove_word(string, word):
    return string.replace(word, "").strip()

print(remove_word("  hello world  ", "world"))

# Input: "  hello world  ", "world"
# Output: hello


# Q8: Multiplication table using function

def table(n):
    for i in range(1, 11):
        print(f"{n} x {i} = {n*i}")

table(3)

# Input: 3
# Output:
# 3 x 1 = 3
# ...
# 3 x 10 = 30
