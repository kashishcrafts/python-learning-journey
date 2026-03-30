# 📘 Chapter 6: Conditional Expressions (if-else)

# 🔹 if statement
a = 10
if a > 5:
    print("a is greater than 5")
# Output: a is greater than 5


# 🔹 if-else statement
a = 3
if a > 5:
    print("Greater")
else:
    print("Smaller")
# Output: Smaller


# 🔹 if-elif-else
marks = 75

if marks >= 90:
    print("Excellent")
elif marks >= 50:
    print("Pass")
else:
    print("Fail")
# Output: Pass


# 🔹 Relational Operators
# >, <, >=, <=, ==, !=

print(5 > 3)    # True
print(5 == 5)   # True
print(5 != 3)   # True


# 🔹 Logical Operators
# and, or, not

a = True
b = False

print(a and b)  # False
print(a or b)   # True
print(not a)    # False


# 🔹 Nested if
age = 20

if age > 18:
    if age < 25:
        print("Young Adult")
# Output: Young Adult


# 🔹 Ternary Operator (one-line if-else)
a = 10
result = "Even" if a % 2 == 0 else "Odd"
print(result)
# Output: Even
