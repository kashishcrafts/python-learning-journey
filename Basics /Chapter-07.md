# 📘 Chapter 7: Loops (Detailed Notes)

# 🔹 What are Loops?
# Loops are used to execute a block of code repeatedly.

# ------------------------------------------
# 🔹 for loop
# Used to iterate over a sequence (list, tuple, string, range)

for i in range(5):
    print(i)
# Output:
# 0 1 2 3 4


# 🔹 range() function
# range(start, stop, step)

print(list(range(5)))        # [0, 1, 2, 3, 4]
print(list(range(1, 6)))     # [1, 2, 3, 4, 5]
print(list(range(1, 10, 2))) # [1, 3, 5, 7, 9]


# 🔹 Loop through string
name = "Kashish"
for ch in name:
    print(ch)
# Output: K a s h i s h


# 🔹 Loop through list
numbers = [10, 20, 30]
for num in numbers:
    print(num)
# Output: 10 20 30


# ------------------------------------------
# 🔹 while loop
# Runs as long as condition is True

i = 1
while i <= 5:
    print(i)
    i += 1
# Output: 1 2 3 4 5


# 🔹 Infinite loop (avoid)
# while True:
#     print("Hello")


# ------------------------------------------
# 🔹 break statement
# Immediately exits the loop

for i in range(10):
    if i == 5:
        break
    print(i)
# Output: 0 1 2 3 4


# ------------------------------------------
# 🔹 continue statement
# Skips current iteration

for i in range(5):
    if i == 2:
        continue
    print(i)
# Output: 0 1 3 4


# ------------------------------------------
# 🔹 pass statement
# Does nothing (placeholder)

for i in range(3):
    pass


# ------------------------------------------
# 🔹 for loop with else
# else executes when loop completes normally

for i in range(3):
    print(i)
else:
    print("Done")
# Output:
# 0 1 2
# Done


# ------------------------------------------
# 🔹 Nested loops
# Loop inside another loop

for i in range(1, 4):
    for j in range(1, 4):
        print(i, j)
# Output:
# (1,1) (1,2) (1,3)
# (2,1) (2,2) (2,3)
# (3,1) (3,2) (3,3)


# ------------------------------------------
# 🔹 Pattern printing example

n = 3
for i in range(1, n+1):
    print("*" * i)
# Output:
# *
# **
# ***


# ------------------------------------------
# 🔹 Difference between for and while

# for loop → fixed iterations
for i in range(3):
    print(i)

# while loop → condition based
i = 0
while i < 3:
    print(i)
    i += 1


# ------------------------------------------
# 🔹 Key Points

# - for loop → used with sequence
# - while loop → condition based
# - break → exit loop
# - continue → skip iteration
# - pass → do nothing
# - else → runs if loop completes normally
