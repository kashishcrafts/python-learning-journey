# 📘 Chapter 13: Advanced Python (Part 2)

# ------------------------------------------
# 🔹 Virtual Environment
# Used to create isolated Python environments

# Create:
# python -m venv myenv

# Activate:
# Windows: myenv\Scripts\activate

# Deactivate:
# deactivate


# ------------------------------------------
# 🔹 pip Freeze
# Shows installed packages

# pip freeze > requirements.txt


# ------------------------------------------
# 🔹 walrus operator (:=)
# Assign and use value in same expression

if (n := 5) > 3:
    print(n)
# Output: 5


# ------------------------------------------
# 🔹 Global Keyword

x = 10

def func():
    global x
    x = 20

func()
print(x)
# Output: 20


# ------------------------------------------
# 🔹 Enumerate Function

lst = ["a", "b", "c"]

for index, value in enumerate(lst):
    print(index, value)

# Output:
# 0 a
# 1 b
# 2 c


# ------------------------------------------
# 🔹 List Methods Advanced

lst = [1, 2, 3]

print(max(lst))   # 3
print(min(lst))   # 1
print(sum(lst))   # 6


# ------------------------------------------
# 🔹 Zip Function

names = ["A", "B", "C"]
marks = [90, 80, 70]

z = list(zip(names, marks))
print(z)

# Output:
# [('A', 90), ('B', 80), ('C', 70)]


# ------------------------------------------
# 🔹 *args and **kwargs

def func(*args):
    print(args)

func(1, 2, 3)
# Output: (1, 2, 3)


def func(**kwargs):
    print(kwargs)

func(a=1, b=2)
# Output: {'a': 1, 'b': 2}


# ------------------------------------------
# 🔹 Docstrings

def add(a, b):
    """This function adds two numbers"""
    return a + b

print(add.__doc__)
# Output: This function adds two numbers


# ------------------------------------------
# 🔹 Main Function (__name__ == "__main__")

def greet():
    print("Hello")

if __name__ == "__main__":
    greet()


# ------------------------------------------
# 🔹 Key Points

# - Virtual env isolates projects
# - walrus operator assigns inline
# - global modifies global variable
# - enumerate gives index + value
# - zip combines lists
# - *args = multiple arguments
# - **kwargs = keyword arguments
