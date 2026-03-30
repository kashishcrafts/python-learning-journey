# Chapter 9 Practice Set - Files

# Q1: Read a file and print its content

with open("sample.txt", "r") as f:
    print(f.read())

# Input: sample.txt contains "Hello Python"
# Output: Hello Python


# Q2: Find if a word exists in file

word = "Python"

with open("sample.txt", "r") as f:
    content = f.read()

if word in content:
    print("Found")
else:
    print("Not Found")

# Input: "Python"
# Output: Found


# Q3: Replace a word in file

with open("sample.txt", "r") as f:
    content = f.read()

content = content.replace("Python", "Java")

with open("sample.txt", "w") as f:
    f.write(content)

# Input: Python
# Output: replaced with Java


# Q4: Write multiplication table to file

n = 5

with open("table.txt", "w") as f:
    for i in range(1, 11):
        f.write(f"{n} x {i} = {n*i}\n")

# Output: table saved in file


# Q5: Copy content from one file to another

with open("sample.txt", "r") as f:
    content = f.read()

with open("copy.txt", "w") as f:
    f.write(content)

# Output: content copied


# Q6: Append data to file

with open("sample.txt", "a") as f:
    f.write("\nNew data added")

# Output: data appended


# Q7: Check file exists

import os

print(os.path.exists("sample.txt"))

# Output: True or False


# Q8: Clear file content

open("sample.txt", "w").close()

# Output: file becomes empty
