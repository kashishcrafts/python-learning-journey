# Chapter 11 Practice Set - Advanced Python

# Q1: Create class with property for name

class Person:
    def __init__(self, name):
        self._name = name

    @property
    def name(self):
        return self._name

p = Person("Kashish")
print(p.name)

# Input: Kashish
# Output: Kashish


# Q2: Add setter for name

class Person:
    def __init__(self, name):
        self._name = name

    @property
    def name(self):
        return self._name

    @name.setter
    def name(self, val):
        self._name = val

p = Person("Kashish")
p.name = "Shaikh"
print(p.name)

# Input: Kashish → Shaikh
# Output: Shaikh


# Q3: Class method to change class attribute

class Demo:
    a = 10

    @classmethod
    def change(cls, val):
        cls.a = val

Demo.change(50)
print(Demo.a)

# Output: 50


# Q4: Static method

class Demo:
    @staticmethod
    def greet():
        print("Hello")

Demo.greet()

# Output: Hello


# Q5: Operator overloading

class Number:
    def __init__(self, num):
        self.num = num

    def __add__(self, other):
        return self.num + other.num

n1 = Number(2)
n2 = Number(3)
print(n1 + n2)

# Output: 5


# Q6: __str__ method

class Demo:
    def __str__(self):
        return "Object Printed"

d = Demo()
print(d)

# Output: Object Printed


# Q7: __len__ method

class Demo:
    def __len__(self):
        return 7

d = Demo()
print(len(d))

# Output: 7
