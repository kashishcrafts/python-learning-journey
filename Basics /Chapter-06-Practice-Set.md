# Chapter 6 Practice Set - Conditional Expressions

# Q1: Find greatest of 3 numbers
a, b, c = 10, 20, 15

if a > b and a > c:
    print("a is greatest")
elif b > c:
    print("b is greatest")
else:
    print("c is greatest")
# Output: b is greatest


# Q2: Check pass or fail
marks = 40

if marks >= 33:
    print("Pass")
else:
    print("Fail")
# Output: Pass


# Q3: Check spam message
text = "Make a lot of money now"

if "money" in text or "buy now" in text:
    print("Spam")
else:
    print("Not Spam")
# Output: Spam


# Q4: Check username length
username = "kashish"

if len(username) < 10:
    print("Valid")
else:
    print("Too long")
# Output: Valid


# Q5: Check name in list
names = ["Kashish", "Rahul", "Aman"]

if "Kashish" in names:
    print("Present")
else:
    print("Not Present")
# Output: Present
