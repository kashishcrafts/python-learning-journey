# 📘 Chapter 7: Loops

# 🔹 for loop
# Used to iterate over a sequence

for i in range(5):
    print(i)
# Output:
# 0
# 1
# 2
# 3
# 4


# 🔹 range() function
# range(start, stop, step)

for i in range(1, 6):
    print(i)
# Output:
# 1 2 3 4 5


# 🔹 while loop
# Runs until condition becomes False

i = 1
while i <= 5:
    print(i)
    i += 1
# Output:
# 1 2 3 4 5


# 🔹 break statement
# Stops the loop immediately

for i in range(10):
    if i == 5:
        break
    print(i)
# Output:
# 0 1 2 3 4


# 🔹 continue statement
# Skips current iteration

for i in range(5):
    if i == 2:
        continue
    print(i)
# Output:
# 0 1 3 4


# 🔹 pass statement
# Does nothing (placeholder)

for i in range(3):
    pass


# 🔹 for loop with else
for i in range(3):
    print(i)
else:
    print("Done")
# Output:
# 0 1 2
# Done
