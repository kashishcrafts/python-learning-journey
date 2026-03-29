# 📘 Chapter 2: Variables & Data Types

## 🔹 Variables
A variable is a name given to a memory location used to store data.

### Example:
```python
a = 10
name = "Kashish"

---

##🔹 Data Types

Python automatically detects the type of data.

Main Data Types:
Integer → int
Float → float
String → str
Boolean → bool
None → NoneType

Example:
a = 10        # int
b = 3.14      # float
name = "Hi"   # string
flag = True   # boolean

---

##🔹 Rules for Variables (Identifiers)

Must start with a letter or underscore
Cannot start with a number
No spaces allowed
No special characters

Correct:
name = "Kashish"
_age = 22

Incorrect:
2name = "error"
my name = "error"

---

##🔹 Operators in Python

Arithmetic Operators:
+  -  *  /

Assignment Operators:
=  +=  -=

Comparison Operators:
==  >  <  >=  <=  !=

Logical Operators:
and  or  not

## 🔹 Logical Operators – Truth Tables

### AND (and)
Returns True only if both conditions are True.

| A     | B     | A and B |
|-------|-------|---------|
| True  | True  | True    |
| True  | False | False   |
| False | True  | False   |
| False | False | False   |

---

### OR (or)
Returns True if at least one condition is True.

| A     | B     | A or B |
|-------|-------|--------|
| True  | True  | True   |
| True  | False | True   |
| False | True  | True   |
| False | False | False  |

---

### NOT (not)
Reverses the value.

| A     | not A |
|-------|-------|
| True  | False |
| False | True  |

---

### 💡 Example in Python
```python
print(True and False)   # False
print(True or False)    # True
print(not True)         # False

---

##🔹 type() Function

Used to check the data type of a variable.

Example:
a = 10
print(type(a))   # <class 'int'>

---

##🔹 Typecasting

Converting one data type into another.

Example:
a = "10"
b = int(a)

print(b)        # 10
print(type(b))  # int

---

##🔹 input() Function

Used to take input from the user.

Example:
name = input("Enter your name: ")
print(name)

---

👉 Note: input() always returns a string

🎯 Summary
Variables store data
Python detects data types automatically
Operators perform operations
type() checks data type
Typecasting converts data types
input() takes user input

---
