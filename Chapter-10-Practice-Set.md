# Chapter 10 Practice Set - OOP 

# Q1: Create class Programmer storing name, salary, language

class Programmer:
    company = "Microsoft"

    def __init__(self, name, salary, language):
        self.name = name
        self.salary = salary
        self.language = language

p = Programmer("Kashish", 100000, "Python")
print(p.name, p.salary, p.language)

# Input: Kashish, 100000, Python
# Output: Kashish 100000 Python


# Q2: Create class Calculator with square, cube, sqrt

class Calculator:
    def square(self, n):
        print(n*n)

    def cube(self, n):
        print(n*n*n)

    def sqrt(self, n):
        print(n**0.5)

c = Calculator()
c.square(4)
c.cube(2)
c.sqrt(16)

# Input: 4, 2, 16
# Output:
# 16
# 8
# 4.0


# Q3: Add static method in Calculator

class Calculator:
    @staticmethod
    def greet():
        print("Hello")

Calculator.greet()

# Output: Hello


# Q4: Create class Train with methods

class Train:
    def __init__(self, name):
        self.name = name

    def book(self):
        print("Ticket booked")

    def getStatus(self):
        print("Train is running")

    def getFare(self):
        print("Fare is 500")

t = Train("Rajdhani")
t.book()
t.getStatus()
t.getFare()

# Output:
# Ticket booked
# Train is running
# Fare is 500


# Q5: Change attribute after object creation

class Sample:
    a = 10

obj = Sample()
obj.a = 20
print(obj.a)

# Output: 20


# Q6: Demonstrate difference between class & instance attribute

class Demo:
    a = 10

obj = Demo()
print(obj.a)   # class attribute

obj.a = 50
print(obj.a)   # instance attribute

# Output:
# 10
# 50
