# Chapter 3 Practice Set - Strings (with outputs)

# Q1: Input name and print greeting
# Input: Kashish
name = "Kashish"
print("Good Afternoon,", name)
# Output: Good Afternoon, Kashish

---

# Q2: Replace double spaces with single space
# Input:
text = "This  is  a  string"
print(text.replace("  ", " "))
# Output: This is a string

---

# Q3: Detect double spaces
# Input:
text = "This  is a string"
print(text.find("  "))
# Output: 4

---

# Q4: Format letter using escape sequences
# Input:
letter = "Dear Kashish,\n\tYou are doing great!\nThanks!"
print(letter)
# Output:
 Dear Kashish,
    You are doing great!
Thanks!

---

# Q5: Slice string
# Input:
name = "Kashish"
print(name[0:3])
# Output: Kas

---

# Q6: Reverse string using slicing
# Input:
print(name[::-1])
# Output: hsihsaK

---

# Q7: Check string starts/ends
# Input:
print(name.startswith("Ka"))
# Output: True

print(name.endswith("sh"))
# Output: True

---
