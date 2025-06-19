# Python-Interview-Questions-
# 🐍 Python Interview Questions

A collection of frequently asked Python interview questions with brief answers and examples. Great for beginners and intermediate developers preparing for interviews.

---

## 📘 Questions & Answers

### 1. What is the difference between List and Tuple in Python?
- **List**: Mutable, uses `[]`, slower, more flexible.
- **Tuple**: Immutable, uses `()`, faster, safer.

---

### 2. How do sets help in removing duplicates?
Using `set(list)` removes duplicates because sets only store unique values.

```python
my_list = [1, 2, 2, 3]
unique = list(set(my_list))  # [1, 2, 3]
3. Why are dictionaries faster than lists for lookups?
Dictionaries use hashing for O(1) average lookup time, while lists use O(n) linear search.
4. How are Python strings immutable if they allow operations like replace()?
Strings are immutable → you can’t change them in-place.

Operations like replace() return a new string.
s = "hello"
new_s = s.replace("h", "y")  # new_s = "yello", s remains "hello"
5. How do you merge two dictionaries in Python (latest version)?
Python 3.9+:
dict1 = {'a': 1}
dict2 = {'b': 2}
merged = dict1 | dict2
6. Explain dictionary comprehension with example
Create a dictionary in a single line:
squares = {x: x*x for x in range(5)}
# Output: {0: 0, 1: 1, 2: 4, 3: 9, 4: 16}
7. What are nested dictionaries and how do you access inner values?
Dictionaries inside dictionaries:
data = {'emp1': {'name': 'John', 'age': 30}}
print(data['emp1']['name'])  # Output: John
8. How can you convert a list of tuples into a dictionary?
lst = [('a', 1), ('b', 2)]
d = dict(lst)
# Output: {'a': 1, 'b': 2}
9. How would you handle a missing key in a dictionary?
Use get() with default:
d = {'a': 1}
print(d.get('b', 0))  # Output: 0
Or use defaultdict from collections
10. Can we use a list as a key in a dictionary? Why/why not?
❌ No, because:

Lists are mutable (changeable).

Only immutable (hashable) types like strings, tuples can be keys.
11. What happens if you try to add a mutable object to a set?
You get a TypeError:
s = set()
s.add([1, 2])  # ❌ TypeError: unhashable type: 'list'
12. Code to find common elements in two lists using set operations
list1 = [1, 2, 3]
list2 = [2, 3, 4]
common = list(set(list1) & set(list2))
# Output: [2, 3]
13. Difference between is and == for strings
== → checks value equality

is → checks object identity (memory)
a = "hello"
b = "hello"
a == b  # ✅ True
a is b  # ✅ True in CPython due to interning (but not guaranteed)
4. How does slicing work in tuple and string? Syntax?
Syntax: obj[start:stop:step]
s = "Python"
t = (1, 2, 3, 4)

print(s[1:4])  # yth
print(t[::2])  # (1, 3)
15. How can you reverse a string or list using slicing?
s = "hello"
print(s[::-1])  # 'olleh'

l = [1, 2, 3]
print(l[::-1])  # [3, 2, 1]







