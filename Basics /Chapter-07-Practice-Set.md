# Chapter 7 Practice Set - Loops

# Q1: Print multiplication table of a number
n = 5
for i in range(1, 11):
    print(f"{n} x {i} = {n*i}")


# Q2: Greet all names in list
names = ["Kashish", "Rahul", "Aman"]

for name in names:
    print("Hello", name)


# Q3: Find if number is prime
n = 7
for i in range(2, n):
    if n % i == 0:
        print("Not Prime")
        break
else:
    print("Prime")


# Q4: Sum of first n natural numbers
n = 5
sum = 0
for i in range(1, n+1):
    sum += i
print(sum)
# Output: 15


# Q5: Factorial of number
n = 5
fact = 1
for i in range(1, n+1):
    fact *= i
print(fact)
# Output: 120
