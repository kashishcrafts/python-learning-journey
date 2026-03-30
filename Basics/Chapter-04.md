# 📘 Chapter 4: Lists & Tuples

## 🔹 Lists
A list is an ordered collection of elements enclosed in square brackets `[]`.

### Example:
```python
marks = [45, 78, 90, 65]
print(marks)

Output:
[45, 78, 90, 65]

---

##🔹 Properties of Lists
Lists are ordered
Lists are mutable
Lists can store different data types
Example:
data = [10, "Kashish", 8.5, True]
print(data)

Output:
[10, 'Kashish', 8.5, True]

---

##🔹 List Indexing

Each element has an index starting from 0.

numbers = [10, 20, 30, 40]
print(numbers[0])
print(numbers[2])

Output:
10
30

---

##🔹 Changing List Elements

Lists are mutable, so values can be changed.

numbers = [10, 20, 30]
numbers[1] = 99
print(numbers)

Output:
[10, 99, 30]

---

##🔹 List Slicing

You can access a part of the list using slicing.

numbers = [10, 20, 30, 40, 50]
print(numbers[1:4])

Output:
[20, 30, 40]

---

##🔹 List Methods

1. append()
Adds an element at the end.

nums = [1, 2, 3]
nums.append(4)
print(nums)

Output:
[1, 2, 3, 4]

2. sort()
Sorts the list.

nums = [4, 1, 3, 2]
nums.sort()
print(nums)

Output:
[1, 2, 3, 4]

3. reverse()
Reverses the list.

nums = [1, 2, 3]
nums.reverse()
print(nums)

Output:
[3, 2, 1]

4. insert()
Inserts element at a specific index.

nums = [1, 3, 4]
nums.insert(1, 2)
print(nums)

Output:
[1, 2, 3, 4]

5. pop()
Removes element from a given index.

nums = [10, 20, 30]
nums.pop(1)
print(nums)

Output:
[10, 30]

6. remove()
Removes the given value.

nums = [1, 2, 3, 2]
nums.remove(2)
print(nums)

Output:
[1, 3, 2]

---

##🔹 Tuples
A tuple is an ordered collection of elements enclosed in parentheses ().

Example:
t = (10, 20, 30)
print(t)

Output:
(10, 20, 30)

---

##🔹 Properties of Tuples
Tuples are ordered
Tuples are immutable
Tuples can store different data types
Example:
t = (1, "Kashish", 7.8, False)
print(t)

Output:
(1, 'Kashish', 7.8, False)

---

##🔹 Tuple Indexing
Tuple indexing works like list indexing.

t = (100, 200, 300)
print(t[0])
print(t[2])

Output:
100
300

---

##🔹 Single Element Tuple
To create a single element tuple, use a comma.

t = (5,)
print(type(t))

Output:
<class 'tuple'>

---

##🔹 Tuple Methods
1. count()
Counts how many times a value appears.

t = (1, 2, 2, 3, 2)
print(t.count(2))

Output:
3

2. index()
Returns the index of first occurrence.

t = (10, 20, 30, 20)
print(t.index(20))

Output:
1

---

🎯 Summary
Lists use [] and are mutable
Tuples use () and are immutable
Indexing starts from 0
Lists support many methods like append, sort, reverse, insert, pop, remove
Tuples support methods like count and index

---
