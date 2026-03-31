# Chapter 12 Practice Set - Advanced Python (Part 1)

# Q1: Handle division by zero

try:
    a = 10 / 0
except ZeroDivisionError:
    print("Cannot divide by zero")

# Output: Cannot divide by zero


# Q2: Create list of squares using list comprehension

lst = [i*i for i in range(1, 6)]
print(lst)

# Output: [1, 4, 9, 16, 25]


# Q3: Filter even numbers

lst = [1, 2, 3, 4, 5]
even = list(filter(lambda x: x%2==0, lst))
print(even)

# Output: [2, 4]


# Q4: Use map to double values

lst = [1, 2, 3]
result = list(map(lambda x: x*2, lst))
print(result)

# Output: [2, 4, 6]


# Q5: Sum using reduce

from functools import reduce

lst = [1, 2, 3, 4]
print(reduce(lambda x, y: x+y, lst))

# Output: 10


# Q6: Raise custom exception

class MyError(Exception):
    pass

try:
    raise MyError("Error occurred")
except MyError as e:
    print(e)

# Output: Error occurred
