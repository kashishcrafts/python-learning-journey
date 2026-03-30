# 📘 Chapter 9: File I/O 

# 🔹 What is File I/O?
# File I/O means reading from and writing to files.

# ------------------------------------------
# 🔹 Opening a File

f = open("file.txt", "r")
# Modes:
# "r" → read
# "w" → write (overwrite)
# "a" → append
# "r+" → read + write

# ------------------------------------------
# 🔹 Reading a File

f = open("file.txt", "r")
data = f.read()
print(data)
f.close()

# Output: content of file


# 🔹 read(n)
f = open("file.txt", "r")
print(f.read(5))  # reads first 5 characters
f.close()


# 🔹 readline()
f = open("file.txt", "r")
print(f.readline())
f.close()


# 🔹 readlines()
f = open("file.txt", "r")
print(f.readlines())
f.close()


# ------------------------------------------
# 🔹 Writing to a File

f = open("file.txt", "w")
f.write("Hello World")
f.close()

# Output: file content replaced


# 🔹 Append Mode

f = open("file.txt", "a")
f.write("\nNew Line")
f.close()

# Output: content added


# ------------------------------------------
# 🔹 Using with statement (BEST PRACTICE)

with open("file.txt", "r") as f:
    data = f.read()
    print(data)

# No need to close file manually


# ------------------------------------------
# 🔹 File Exists Check

import os

if os.path.exists("file.txt"):
    print("File exists")
else:
    print("File not found")


# ------------------------------------------
# 🔹 Key Points

# - Always close file after use
# - 'with' automatically closes file
# - 'w' overwrites file
# - 'a' appends data
# - 'r' reads file

-----
