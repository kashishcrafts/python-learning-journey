# 📘 Chapter 10: Object Oriented Programming 

# 🔹 What is OOP?
# OOP (Object Oriented Programming) is a programming paradigm based on classes and objects.
# It helps in organizing code and making it reusable.

# ------------------------------------------
# 🔹 Class
# A class is a blueprint for creating objects.

class Employee:
    company = "Google"

# ------------------------------------------
# 🔹 Object
# An object is an instance of a class.

emp1 = Employee()
print(emp1.company)
# Output: Google


# ------------------------------------------
# 🔹 Attributes
# Data inside a class

class Employee:
    company = "Google"   # class attribute

    def __init__(self, name, salary):
        self.name = name      # instance attribute
        self.salary = salary

emp = Employee("Kashish", 100000)
print(emp.name, emp.salary)


# ------------------------------------------
# 🔹 __init__ Method (Constructor)
# Automatically called when object is created

class Student:
    def __init__(self, name):
        self.name = name

s = Student("Kashish")
print(s.name)


# ------------------------------------------
# 🔹 Methods
# Functions defined inside class

class Demo:
    def greet(self):
        print("Hello")

d = Demo()
d.greet()


# ------------------------------------------
# 🔹 self Keyword
# Refers to current object

class Test:
    def show(self):
        print(self)

t = Test()
t.show()


# ------------------------------------------
# 🔹 Static Method
# Does not depend on instance

class Demo:
    @staticmethod
    def hello():
        print("Hello World")

Demo.hello()


# ------------------------------------------
# 🔹 Inheritance
# One class inherits properties of another

class Parent:
    def show(self):
        print("Parent class")

class Child(Parent):
    pass

c = Child()
c.show()


# ------------------------------------------
# 🔹 Method Overriding

class Parent:
    def show(self):
        print("Parent")

class Child(Parent):
    def show(self):
        print("Child")

c = Child()
c.show()


# ------------------------------------------
# 🔹 super() Keyword

class Parent:
    def __init__(self):
        print("Parent constructor")

class Child(Parent):
    def __init__(self):
        super().__init__()
        print("Child constructor")

c = Child()


# ------------------------------------------
# 🔹 Class vs Instance Attributes

class Demo:
    a = 10   # class attribute

obj = Demo()
obj.a = 20  # instance overrides
print(obj.a)   # 20


# ------------------------------------------
# 🔹 Key Points

# - Class = blueprint
# - Object = instance
# - __init__ = constructor
# - self = current object
# - Inheritance = reuse code
# - Overriding = change method behavior
# - Static method = no self
