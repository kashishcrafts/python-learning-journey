# Chapter 13 Practice Set - Advanced Python

# Q1: Use enumerate

lst = ["apple", "banana", "mango"]

for i, val in enumerate(lst):
    print(i, val)

# Output:
# 0 apple
# 1 banana
# 2 mango


# Q2: Use zip

names = ["A", "B"]
marks = [50, 60]

print(list(zip(names, marks)))

# Output: [('A', 50), ('B', 60)]


# Q3: Use *args

def add(*nums):
    print(sum(nums))

add(1, 2, 3)

# Output: 6


# Q4: Use **kwargs

def show(**data):
    print(data)

show(name="Kashish", age=22)

# Output: {'name': 'Kashish', 'age': 22}


# Q5: Use docstring

def greet():
    """This function greets user"""
    pass

print(greet.__doc__)

# Output: This function greets user


# Q6: Walrus operator

if (x := 10) > 5:
    print(x)

# Output: 10
