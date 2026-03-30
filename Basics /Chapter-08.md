# 📘 Chapter 8: Functions

# 🔹 What is a Function?
# A function is a block of code that performs a specific task.

# 🔹 Why use functions?
# - Avoid repetition
# - Makes code reusable
# - Improves readability

# ------------------------------------------
# 🔹 Function Definition & Call

def greet():
    print("Hello!")

greet()
# Output: Hello!


# ------------------------------------------
# 🔹 Function with Parameters

def greet(name):
    print("Hello", name)

greet("Kashish")
# Output: Hello Kashish


# ------------------------------------------
# 🔹 Function with Return Value

def add(a, b):
    return a + b

result = add(10, 5)
print(result)
# Output: 15


# ------------------------------------------
# 🔹 Default Arguments

def greet(name="User"):
    print("Hello", name)

greet()
# Output: Hello User

greet("Kashish")
# Output: Hello Kashish


# ------------------------------------------
# 🔹 Keyword Arguments

def intro(name, age):
    print(name, age)

intro(age=22, name="Kashish")
# Output: Kashish 22


# ------------------------------------------
# 🔹 Recursion
# Function calling itself

def factorial(n):
    if n == 1 or n == 0:
        return 1
    return n * factorial(n-1)

print(factorial(5))
# Output: 120


# ------------------------------------------
# 🔹 Local vs Global Variables

x = 10  # global

def func():
    x = 5  # local
    print(x)

func()   # 5
print(x) # 10


# ------------------------------------------
# 🔹 pass statement

def empty():
    pass


# ------------------------------------------
# 🔹 Key Points

# - def keyword is used to define function
# - return gives result back
# - parameters are inputs
# - functions can be reused
# - recursion = function calling itself
