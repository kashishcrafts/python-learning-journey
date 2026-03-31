# 📘 Chapter 12: Advanced Python (Part 1)

# ------------------------------------------
# 🔹 Exception Handling

# Used to handle runtime errors

try:
    a = int("abc")   # error
except Exception as e:
    print("Error occurred:", e)

# Output: Error occurred


# ------------------------------------------
# 🔹 try-except-else

try:
    a = int("10")
except:
    print("Error")
else:
    print("Success")

# Output: Success


# ------------------------------------------
# 🔹 finally block

try:
    print("Try block")
finally:
    print("Always executed")

# Output:
# Try block
# Always executed


# ------------------------------------------
# 🔹 Raising Exceptions

a = 5
if a < 10:
    raise ValueError("Value is less than 10")


# ------------------------------------------
# 🔹 Custom Exception

class MyError(Exception):
    pass

try:
    raise MyError("Custom Error")
except MyError as e:
    print(e)

# Output: Custom Error


# ------------------------------------------
# 🔹 File Handling (Advanced)

with open("file.txt", "w") as f:
    f.write("Hello")


# ------------------------------------------
# 🔹 List Comprehension

lst = [i for i in range(5)]
print(lst)
# Output: [0, 1, 2, 3, 4]


# With condition
lst = [i for i in range(10) if i % 2 == 0]
print(lst)
# Output: [0, 2, 4, 6, 8]


# ------------------------------------------
# 🔹 Dictionary Comprehension

d = {i: i*i for i in range(5)}
print(d)
# Output: {0:0, 1:1, 2:4, 3:9, 4:16}


# ------------------------------------------
# 🔹 Set Comprehension

s = {i for i in range(5)}
print(s)
# Output: {0,1,2,3,4}


# ------------------------------------------
# 🔹 Lambda Functions

square = lambda x: x*x
print(square(5))
# Output: 25


# ------------------------------------------
# 🔹 Map Function

lst = [1, 2, 3]
result = list(map(lambda x: x*x, lst))
print(result)
# Output: [1, 4, 9]


# ------------------------------------------
# 🔹 Filter Function

lst = [1, 2, 3, 4]
result = list(filter(lambda x: x%2==0, lst))
print(result)
# Output: [2, 4]


# ------------------------------------------
# 🔹 Reduce Function

from functools import reduce

lst = [1, 2, 3, 4]
result = reduce(lambda x, y: x+y, lst)
print(result)
# Output: 10


# ------------------------------------------
# 🔹 Key Points

# - try/except handles errors
# - finally always executes
# - list/dict/set comprehension = short syntax
# - lambda = small anonymous function
# - map/filter/reduce = functional programming tools
