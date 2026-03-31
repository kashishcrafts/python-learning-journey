# 📘 Chapter 11: Advanced Python (Properties, Decorators, etc.)

# ------------------------------------------
# 🔹 Property Decorator (@property)
# Used to define a method as an attribute

class Employee:
    def __init__(self, salary):
        self._salary = salary

    @property
    def salary(self):
        return self._salary

e = Employee(50000)
print(e.salary)
# Output: 50000


# ------------------------------------------
# 🔹 Setter (@<property>.setter)

class Employee:
    def __init__(self, salary):
        self._salary = salary

    @property
    def salary(self):
        return self._salary

    @salary.setter
    def salary(self, value):
        self._salary = value

e = Employee(50000)
e.salary = 60000
print(e.salary)
# Output: 60000


# ------------------------------------------
# 🔹 Class Method (@classmethod)

class Demo:
    a = 10

    @classmethod
    def change(cls, val):
        cls.a = val

Demo.change(20)
print(Demo.a)
# Output: 20


# ------------------------------------------
# 🔹 Static Method (@staticmethod)

class Demo:
    @staticmethod
    def greet():
        print("Hello")

Demo.greet()


# ------------------------------------------
# 🔹 Operator Overloading

class Number:
    def __init__(self, num):
        self.num = num

    def __add__(self, other):
        return self.num + other.num

n1 = Number(5)
n2 = Number(10)
print(n1 + n2)
# Output: 15


# ------------------------------------------
# 🔹 __str__ Method

class Demo:
    def __str__(self):
        return "This is object"

d = Demo()
print(d)
# Output: This is object


# ------------------------------------------
# 🔹 __len__ Method

class Demo:
    def __len__(self):
        return 5

d = Demo()
print(len(d))
# Output: 5


# ------------------------------------------
# 🔹 Getter, Setter Concept
# Encapsulation using property

class Student:
    def __init__(self, marks):
        self._marks = marks

    def get_marks(self):
        return self._marks

    def set_marks(self, val):
        self._marks = val


# ------------------------------------------
# 🔹 Key Points

# - @property → method ko attribute jaisa use karte hain
# - setter → value change karne ke liye
# - classmethod → class level change
# - staticmethod → independent method
# - operator overloading → + ko redefine karna
# - __str__ → print object behavior
# - __len__ → length define karna
