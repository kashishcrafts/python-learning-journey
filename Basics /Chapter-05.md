# 📘 Chapter 5: Dictionary & Sets (Notes)

# 🔹 Dictionary
# A dictionary is a collection of key-value pairs

student = {
    "name": "Kashish",
    "marks": 90,
    "age": 22
}
print(student)

# Output: {'name': 'Kashish', 'marks': 90, 'age': 22}

---

# 🔹 Accessing values
print(student["name"])

# Output: Kashish

---

# 🔹 Properties of Dictionary
# - Unordered
# - Mutable
# - Keys are unique

---

# 🔹 Dictionary Methods

d = {"a": 1, "b": 2}

print(d.keys())

# Output: dict_keys(['a', 'b'])

print(d.values())

# Output: dict_values([1, 2])

print(d.items())

# Output: dict_items([('a', 1), ('b', 2)])

d.update({"c": 3})
print(d)

# Output: {'a': 1, 'b': 2, 'c': 3}

print(d.get("a"))

# Output: 1

---

# 🔹 Sets
# A set is an unordered collection of unique elements

s = {1, 2, 3, 3}
print(s)

# Output: {1, 2, 3}

---

# 🔹 Properties of Sets
# - Unordered
# - No duplicates
# - Mutable

---

# 🔹 Set Methods

s.add(4)
print(s)
# Output: {1, 2, 3, 4}

s.remove(2)
print(s)
# Output: {1, 3, 4}

a = {1, 2}
b = {2, 3}

print(a.union(b))
# Output: {1, 2, 3}

print(a.intersection(b))
# Output: {2}

---
