# 📘 Chapter 3: Strings

## 🔹 What is a String?
A string is a sequence of characters enclosed in quotes.

### Example:
```python
name = "Kashish"

---

##🔹 String Indexing

Each character in a string has an index.

name = "Kashish"
K	a	s	h	i	s	h
0	1	2	3	4	5	6

👉 Negative indexing:
| -7 | -6 | -5 | -4 | -3 | -2 | -1 |

---

##🔹 String Slicing
name = "Kashish"
print(name[0:3])  # Kas

👉 Format:

string[start:end]
---

##🔹 Slicing with Skip Value
name = "Kashish"
print(name[0:7:2])  # Kshh

👉 Format:

string[start:end:step]

---

##🔹 String Functions
name = "kashish"
print(len(name))        # length
print(name.endswith("sh"))  
print(name.startswith("ka"))  
print(name.capitalize())  
print(name.upper())  
print(name.lower())  
print(name.find("sh"))  
print(name.replace("ka", "ra"))

---
 
##🔹 Escape Sequence Characters

Used to format strings.

print("Hello\nWorld")   # new line
print("Hello\tWorld")   # tab space
print("Hello \"World\"")  # quotes inside string

---

🎯 Summary
Strings are sequences of characters
Indexing starts from 0
Slicing extracts parts of string
Functions modify strings
Escape sequences format output

---
